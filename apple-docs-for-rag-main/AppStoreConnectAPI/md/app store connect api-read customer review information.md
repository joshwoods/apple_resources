

- App Store Connect API
-  Read Customer Review Information 

Web Service Endpoint

# Read Customer Review Information

Get information about a specific customer review, including the review content.

App Store Connect API 2.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/customerReviews/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The resource ID representing a unique customer review.

## Query Parameters

`fields[customerReviewResponses]`

`[string]`

Fields to return for included related `customerReviewResponses` resources.

Possible Values: `responseBody, lastModifiedDate, state, review`

`fields[customerReviews]`

`[string]`

Fields to return for included related `customerReviews` resources.

Possible Values: `rating, title, body, reviewerNickname, createdDate, territory, response`

`include`

`[string]`

Relationship data to include in the response.

Value: `response`

## Response Codes

` 200 ``OK`

CustomerReviewResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

An error occurred with your request.

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Request not authorized.

Content-Type: application/json

` 404 ``Not Found`

ErrorResponse

`Not Found`

Resource not found.

Content-Type: application/json

