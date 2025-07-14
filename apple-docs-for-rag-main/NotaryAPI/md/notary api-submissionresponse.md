

- Notary API
-  SubmissionResponse 

Object

# SubmissionResponse

The notary service’s response to a request for the status of a submission.

Notary API 2.0.0+

``` source
object SubmissionResponse
```

## Properties

`data`

SubmissionResponse.Data

Data that describes the status of the submission request.

`meta`

SubmissionResponse.Meta

An empty object that you can ignore.

## Attributes 

Possible types:

## Discussion

You receive a structure of this type in response to a call to the Get Submission Status endpoint.

## Topics

### Objects

object SubmissionResponse.Data

Information that the service provides about the status of a notarization submission.

object SubmissionResponse.Meta

An empty object.

## See Also

### Notarization results

Get Submission Status

Fetch the status of a software notarization submission.

Get Submission Log

Fetch details about a single completed notarization.

object SubmissionLogURLResponse

The notary service’s response to a request for the log information about a completed submission.

