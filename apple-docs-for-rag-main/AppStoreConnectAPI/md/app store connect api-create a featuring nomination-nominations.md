

- App Store Connect API
-  Create a featuring nomination 

Web Service Endpoint

# Create a featuring nomination

Tell Apple about your upcoming app or feature.

App Store Connect API 3.8+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/nominations
```

## HTTP Body

NominationCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

NominationResponse

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

### Managing nominations

List nominations

Get all featuring nominations.

Read details for a nomination

Get information for a specific featuring nomination.

Modify a nomination

Update a specific featuring nomination.

Delete a featuring nomination

Remove a specific featuring nomination.

