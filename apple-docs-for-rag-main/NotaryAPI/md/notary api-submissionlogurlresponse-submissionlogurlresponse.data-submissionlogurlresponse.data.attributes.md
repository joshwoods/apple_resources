

- Notary API
- SubmissionLogURLResponse
- SubmissionLogURLResponse.Data
-  SubmissionLogURLResponse.Data.Attributes 

Object

# SubmissionLogURLResponse.Data.Attributes

Information about the log associated with the submission.

Notary API 2.0.0+

``` source
object SubmissionLogURLResponse.Data.Attributes
```

## Properties

`developerLogUrl`

`string`

The URL that you use to download the logs for a submission. The URL serves a JSON-encoded file that contains the log information. The URL is valid for only a few hours. If you need the log again later, ask for the URL again by making another call to the Get Submission Log endpoint.

## Attributes 

Possible types:

