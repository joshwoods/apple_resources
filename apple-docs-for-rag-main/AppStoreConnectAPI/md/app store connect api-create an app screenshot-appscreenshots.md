

- App Store Connect API
-  Create an App Screenshot 

Web Service Endpoint

# Create an App Screenshot

Add a new screenshot to a screenshot set.

App Store Connect API 1.2+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/appScreenshots
```

## HTTP Body

AppScreenshotCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

AppScreenshotResponse

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

The provided resource data is not valid.

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## See Also

### Creating, Modifying, and Deleting Screenshots

Modify an App Screenshot

Commit an app screenshot after uploading it.

Delete an App Screenshot

Delete an app screenshot that is associated with a screenshot set.

