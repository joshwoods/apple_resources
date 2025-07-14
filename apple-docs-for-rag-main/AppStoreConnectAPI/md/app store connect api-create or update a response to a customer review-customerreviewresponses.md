

- App Store Connect API
-  Create or Update a Response to a Customer Review 

Web Service Endpoint

# Create or Update a Response to a Customer Review

Create a response or replace an existing response you wrote to a customer review.

App Store Connect API 2.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/customerReviewResponses
```

## HTTP Body

CustomerReviewResponseV1CreateRequest

The request body of the customer review response.

Content-Type: application/json

## Response Codes

` 201 ``Created`

CustomerReviewResponseV1Response

`Created`

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

The provided resource data isn’t valid.

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## Discussion

Use this endpoint to create a response to a customer review and publish it in the App Store. If a response already exists, this endpoint updates the response by overwriting it.

Responses don’t appear in the App Store instantly. Allow some time for the App Store to publish the response.

## See Also

### Creating, Updating, and Deleting Review Responses

Delete a Response to a Customer Review

Delete a specific response you wrote to a customer review.

