

- Notary API
-  Get Submission Status 

Web Service Endpoint

# Get Submission Status

Fetch the status of a software notarization submission.

Notary API 2.0.0+

## URL

``` source
GET https://appstoreconnect.apple.com/notary/v2/submissions/{submissionId}
```

## Path Parameters

`submissionId`

`uuid`

 (Required) 

The identifier that you receive from the notary service when you post to Submit Software to start a new submission.

Value: `/[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}/`

## Response Codes

` 200 ``OK`

SubmissionResponse

`OK`

The status request succeeded. The response contains the status.

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

An authentication failure occurred.

Content-Type: application/json

` 404 ``Not Found`

ErrorResponse

`Not Found`

The specified identifier can’t be found.

Content-Type: application/json

## Mentioned in 

Submitting software for notarization over the web

## Discussion

Use this endpoint to fetch the status of a submission request. Form the URL for the call using the identifier that you receive in the `id` field of the response to the Submit Software endpoint. If you lose the identifier, you can get a list of the most recent 100 submissions by calling the Get Previous Submissions endpoint.

Along with the status of the request, the response indicates the date that you initiated the request and the software name that you provided at that time.

### Example

- Request
- Response

```
https://appstoreconnect.apple.com/notary/v2/submissions/2efe2717-52ef-43a5-96dc-0797e4ca1041
```

```
{
  "data": {
    "attributes": {
      "createdDate": "2022-06-08T01:38:09.498Z",
      "name": "OvernightTextEditor_11.6.8.zip",
      "status": "Accepted"
    },
    "id": "2efe2717-52ef-43a5-96dc-0797e4ca1041",
    "type": "submissions"
  },
  "meta": {
  }
} 
```

## See Also

### Notarization results

object SubmissionResponse

The notary service’s response to a request for the status of a submission.

Get Submission Log

Fetch details about a single completed notarization.

object SubmissionLogURLResponse

The notary service’s response to a request for the log information about a completed submission.

