

- Notary API
-  NewSubmissionResponse 

Object

# NewSubmissionResponse

The notary service’s response to a software submission.

Notary API 2.0.0+

``` source
object NewSubmissionResponse
```

## Properties

`data`

NewSubmissionResponse.Data

Data that describes the result of the submission request.

`meta`

NewSubmissionResponse.Meta

An empty object that you can ignore.

## Attributes 

Possible types:

## Discussion

You receive a structure of this type in response to a call to the Submit Software endpoint. Use the temporary security credentials this response contains to make a call to Amazon S3 to upload your software.

## Topics

### Objects

object NewSubmissionResponse.Data

Information that the notary service provides for uploading your software for notarization and tracking the submission.

object NewSubmissionResponse.Meta

An empty object.

## See Also

### Software submission

Submit Software

Start the process of uploading a new version of your software to the notary service.

object NewSubmissionRequest

Data that you provide when starting a submission to the notary service.

