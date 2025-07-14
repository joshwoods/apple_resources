

- Notary API
- NewSubmissionResponse
-  NewSubmissionResponse.Data 

Object

# NewSubmissionResponse.Data

Information that the notary service provides for uploading your software for notarization and tracking the submission.

Notary API 2.0.0+

``` source
object NewSubmissionResponse.Data
```

## Properties

`attributes`

NewSubmissionResponse.Data.Attributes

Information that you use to upload your software to Amazon S3.

`id`

`string`

A unique identifier for this submission. Use this value to track the status of your submission. For example, you use it as the `submissionID` parameter in the Get Submission Status call, or to match against the `id` field in the response from the Get Previous Submissions call.

`type`

`string`

The resource type.

## Attributes 

Possible types:

## Topics

### Objects

object NewSubmissionResponse.Data.Attributes

Information that you use to upload your software for notarization.

## See Also

### Objects

object NewSubmissionResponse.Meta

An empty object.

