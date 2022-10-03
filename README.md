# s3-uploader

Watches a folder and upload contents to an s3 bucket of your choice. 


### Pre-requisites

- You need to have valid aws credentials in your path. How? [HERE](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-quickstart.html)
- You need to have at least `PutObject` permission to the bucket.
- Make sure that the bucket you're uploading to or wanting to create is in your local region, otherwise upload will be extremely slow.

## Getting started

A small cli that watches a folder and uploads every change to s3

1. Install via npm `npm install s3-uploader -g`
2. Usage: `s3-uploader -b my-bucket -d ./my-folder` (You can also just go `s3-uploader` auto prompt will guide you through)

If the folder is new, the cli will ask if you want to create one

## Options

```sh
-r -region  # region you're uploading to.
-d -dir     # directory to be watched
-b -bucket  # bucket name to upload to
```

---