# lambdaJSResize

## deployed site
-[http://taskmaster-frontend-jack.s3-website-us-west-2.amazonaws.com/](http://taskmaster-frontend-jack.s3-website-us-west-2.amazonaws.com/)

## how to use the lambda
this lambda fires automatically on uploading a file to the s3 bucket taskmaster-pictures.  once fired, the event triggers and a copy of the resized image moves to taskmaster-pictures-resized.

## images
![S3 picture bucket](/taskmaster-pictures.png)
![S3 resized bucket](/taskmaster-pictures-resized.png)

![cloudwatch logs](/cloud.png)

## known issues:
- the node environment must be set to 8.10 or the function will fail 
- cloudwatch logs are great, but you'll have to look through a tiny screen for the right line to help you.
- the naming convention uses the source file to find the next bucket, so take that into consideration.
- the actual code (to make sure it works) is hard to test on the JS side, because it relies on a working example to confirm.

## credits and contributions
- https://memorynotfound.com/java-resize-image-fixed-width-height-example/
- @Bomibear
- Nhu Trinh
- Matt Stuhring
- Padma GannaPathi
- Renee Messick
- Jane Hur
- Travis Cox
  