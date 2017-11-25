My personal website and resume hosted within S3.

## Compiling css
```sass --watch css/main.scss:css/main.css --style compressed```

## Uploading to S3
```aws s3 cp . s3:///itsmattburgess.co.uk --recursive --exclude ".*" --exclude "*/.sass-cache/*" --storage-class=REDUCED_REDUNDANCY --sse --acl=public-read```
