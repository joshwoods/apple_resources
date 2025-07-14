

- App Store Connect API
-  Read Customer Review Response Information 

Web Service Endpoint

# Read Customer Review Response Information

Get information about a specific response you wrote to a customer review, including the response content and its state.

App Store Connect API 2.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/customerReviewResponses/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies a `customerReviewResponses` resource that represents your review response.

## Query Parameters

`fields[customerReviewResponses]`

`[string]`

Fields to return for the included related types.

Possible Values: `responseBody, lastModifiedDate, state, review`

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

Get a Customer Review Response

Get the response to a specific customer review.

