

- App Store Connect API
-  PATCH /v1/reviewSubmissionItems/{id} 

Web Service Endpoint

# PATCH /v1/reviewSubmissionItems/{id}

App Store Connect API 1.7+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/reviewSubmissionItems/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## HTTP Body

ReviewSubmissionItemUpdateRequest

Content-Type: application/json

## Response Codes

` 200 ``OK`

ReviewSubmissionItemResponse

`OK`

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

` 404 ``Not Found`

ErrorResponse

`Not Found`

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

POST /v1/reviewSubmissionItems

Remove a Review Submission Item

Remove a specific item from a review submission.

