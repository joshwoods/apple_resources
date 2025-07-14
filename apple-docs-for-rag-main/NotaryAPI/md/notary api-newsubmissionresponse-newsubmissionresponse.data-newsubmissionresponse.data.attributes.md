

- Notary API
- NewSubmissionResponse
- NewSubmissionResponse.Data
-  NewSubmissionResponse.Data.Attributes 

Object

# NewSubmissionResponse.Data.Attributes

Information that you use to upload your software for notarization.

Notary API 2.0.0+

``` source
object NewSubmissionResponse.Data.Attributes
```

## Properties

`awsAccessKeyId`

`string`

An access key that you use in a call to Amazon S3.

`awsSecretAccessKey`

`string`

A secret key that you use in a call to Amazon S3.

`awsSessionToken`

`string`

A session token that you use in a call to Amazon S3.

`bucket`

`string`

The Amazon S3 bucket that you upload your software into.

`object`

`string`

The object key that identifies your software upload within the bucket.

## Attributes 

Possible types:

## Discussion

Use the temporary security credentials in this object, along with the bucket and object, to upload your software to Amazon S3. A good way to do this is with the `boto3` library provided by Amazon, as described in Submitting software for notarization over the web. Be sure to use the S3 credentials before they expire, which happens 12 hours after you receive them.

For more information about using this library and accessing Amazon S3, see the documentation on https://aws.amazon.com.

