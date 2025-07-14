

- App Store Connect API
-  Remove a Review Submission Item 

Web Service Endpoint

# Remove a Review Submission Item

Remove a specific item from a review submission.

App Store Connect API 1.7+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/reviewSubmissionItems/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Response Codes

` 204 ``No Content`

`No Content`

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

` 404 ``Not Found`

ErrorResponse

`Not Found`

Content-Type: application/json

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

## See Also

### Endpoints

PATCH /v1/reviewSubmissionItems/{id}

POST /v1/reviewSubmissionItems

