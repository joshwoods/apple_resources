

- App Store Connect API
-  Get a Customer Review Response 

Web Service Endpoint

# Get a Customer Review Response

Get the response to a specific customer review.

App Store Connect API 2.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/customerReviews/{id}/response
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies a `customerReviews` resource that represents a customer review. For more information, see Customer Reviews.

## Query Parameters

`fields[customerReviewResponses]`

`[string]`

Fields to return for included related types.

Possible Values: `responseBody, lastModifiedDate, state, review`

`fields[customerReviews]`

`[string]`

Fields to return for included related types.

Possible Values: `rating, title, body, reviewerNickname, createdDate, territory, response`

`include`

`[string]`

Relationship data to include in the response.

Value: `review`

## Response Codes

` 200 ``OK`

CustomerReviewResponseV1Response

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

## See Also

### Getting Review Responses

Read Customer Review Response Information

Get information about a specific response you wrote to a customer review, including the response content and its state.

