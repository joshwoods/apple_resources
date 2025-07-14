

- Notary API
-  SubmissionLogURLResponse 

Object

# SubmissionLogURLResponse

The notary service’s response to a request for the log information about a completed submission.

Notary API 2.0.0+

``` source
object SubmissionLogURLResponse
```

## Properties

`data`

SubmissionLogURLResponse.Data

Data that indicates how to get the log information for a particular submission.

`meta`

SubmissionLogURLResponse.Meta

An empty object that you can ignore.

## Attributes 

Possible types:

## Discussion

You receive a structure of this type in response to a call to the Get Submission Log endpoint.

## Topics

### Objects

object SubmissionLogURLResponse.Data

Data that indicates how to get the log information for a particular submission.

object SubmissionLogURLResponse.Meta

An empty object.

## See Also

### Notarization results

Get Submission Status

Fetch the status of a software notarization submission.

object SubmissionResponse

The notary service’s response to a request for the status of a submission.

Get Submission Log

Fetch details about a single completed notarization.

