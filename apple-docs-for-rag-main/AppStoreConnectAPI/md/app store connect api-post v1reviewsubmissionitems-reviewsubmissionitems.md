

- App Store Connect API
-  POST /v1/reviewSubmissionItems 

Web Service Endpoint

# POST /v1/reviewSubmissionItems

App Store Connect API 1.7+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/reviewSubmissionItems
```

## HTTP Body

ReviewSubmissionItemCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

ReviewSubmissionItemResponse

`Created`

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Content-Type: application/json

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## See Also

### Endpoints

PATCH /v1/reviewSubmissionItems/{id}

Remove a Review Submission Item

Remove a specific item from a review submission.

