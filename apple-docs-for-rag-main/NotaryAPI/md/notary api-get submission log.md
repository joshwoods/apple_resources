

- Notary API
-  Get Submission Log 

Web Service Endpoint

# Get Submission Log

Fetch details about a single completed notarization.

Notary API 2.0.0+

## URL

``` source
GET https://appstoreconnect.apple.com/notary/v2/submissions/{submissionId}/logs
```

## Path Parameters

`submissionId`

`string`

 (Required) 

The identifier that you receive from the notary service when you post to Submit Software to start a new submission.

## Response Codes

` 200 ``OK`

SubmissionLogURLResponse

`OK`

The request succeeded. The response contains a URL that you access to download the log information.

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

An authentication failure occurred.

Content-Type: application/json

` 404 ``Not Found`

ErrorResponse

`Not Found`

No data was found for this team.

Content-Type: application/json

## Mentioned in 

Submitting software for notarization over the web

## Discussion

Use this endpoint to get a URL that you can download a log file from that enumerates any issues found by the notary service. The URL that you receive is temporary, so be sure to use it to immediately fetch the log. If you need the log again in the future, ask for the URL again.

The log file that you download contains JSON-formatted data, and might include both errors and warnings. For information about how to deal with common notarization problems, see Resolving common notarization issues.

### Example

- Request
- Response

```
https://appstoreconnect.apple.com/notary/v2/submissions/2EFE2717-52EF-43A5-96DC-0797E4CA1041/logs
```

```
{
  "data": {
    "attributes": {
      "developerLogUrl": "https://..."
    },
    "id": "2efe2717-52ef-43a5-96dc-0797e4ca1041",
    "type": "submissionsLog"
  },
  "meta": {
  }
} 

```

## See Also

### Notarization results

Get Submission Status

Fetch the status of a software notarization submission.

object SubmissionResponse

The notary service’s response to a request for the status of a submission.

object SubmissionLogURLResponse

The notary service’s response to a request for the log information about a completed submission.

