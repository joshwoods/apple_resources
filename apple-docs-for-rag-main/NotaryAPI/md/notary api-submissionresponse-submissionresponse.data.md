

- Notary API
- SubmissionResponse
-  SubmissionResponse.Data 

Object

# SubmissionResponse.Data

Information that the service provides about the status of a notarization submission.

Notary API 2.0.0+

``` source
object SubmissionResponse.Data
```

## Properties

`attributes`

SubmissionResponse.Data.Attributes

Information about the status of a submission.

`id`

`string`

The unique identifier for this submission. This value matches the value that you provided as a path parameter to the Get Submission Status call that elicited this response.

`type`

`string`

The resource type.

## Attributes 

Possible types:

## Topics

### Objects

object SubmissionResponse.Data.Attributes

Information about the status of a submission.

## See Also

### Objects

object SubmissionResponse.Meta

An empty object.

