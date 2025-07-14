

- Notary API
-  Get Previous Submissions 

Web Service Endpoint

# Get Previous Submissions

Fetch a list of your team’s previous notarization submissions.

Notary API 2.0.0+

## URL

``` source
GET https://appstoreconnect.apple.com/notary/v2/submissions
```

## Response Codes

` 200 ``OK`

SubmissionListResponse

`OK`

The submission list request succeeded. The response contains a list of recent submissions, truncated to the 100 most recent.

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

Use this endpoint to get the list of submissions associated with your team. The response holds an array of values that include the unique identifier for the submission, the date you initiated the submission, the name of the associated software, and the status of the submission. The response returns information about only the 100 most recent submissions.

If you need information about just one submission, and you have the associated identifier, use Get Submission Status instead.

### Example

- Request
- Response

```
```

```
```

## See Also

### History

object SubmissionListResponse

The notary service’s response to a request for information about your team’s previous submissions.

