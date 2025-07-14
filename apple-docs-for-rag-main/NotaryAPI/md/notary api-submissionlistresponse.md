

- Notary API
-  SubmissionListResponse 

Object

# SubmissionListResponse

The notary service’s response to a request for information about your team’s previous submissions.

Notary API 2.0.0+

``` source
object SubmissionListResponse
```

## Properties

`data`

`[`SubmissionListResponse.Data`]`

An array of objects, each of which describes one of your team’s previous submissions.

`meta`

SubmissionListResponse.Meta

An empty object that you can ignore.

## Attributes 

Possible types:

## Discussion

You receive a structure of this type in response to a call to the Get Previous Submissions endpoint. The list includes only the 100 most recent submissions.

## Topics

### Objects

object SubmissionListResponse.Data

Data that describes one of your team’s previous submissions.

object SubmissionListResponse.Meta

An empty object.

## See Also

### History

Get Previous Submissions

Fetch a list of your team’s previous notarization submissions.

