

- App Store Connect API
-  Delete a Response to a Customer Review 

Web Service Endpoint

# Delete a Response to a Customer Review

Delete a specific response you wrote to a customer review.

App Store Connect API 2.0+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/customerReviewResponses/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies a `customerReviewResponses` resource that represents your review response.

## Response Codes

` 204 ``No Content`

`No Content`

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

The provided resource data isn’t valid.

Content-Type: application/json

## Discussion

Deletions of responses don’t take effect instantly in the App Store. Allow some time for the deletion to take effect.

## See Also

### Creating, Updating, and Deleting Review Responses

Create or Update a Response to a Customer Review

Create a response or replace an existing response you wrote to a customer review.

