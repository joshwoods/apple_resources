

- App Store Connect API
-  Create an App Screenshot Set 

Web Service Endpoint

# Create an App Screenshot Set

Add a new screenshot set to an App Store version localization for a specific screenshot type and display size.

App Store Connect API 1.2+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/appScreenshotSets
```

## HTTP Body

AppScreenshotSetCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

AppScreenshotSetResponse

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

### Creating and Deleting Screenshot Sets

Delete an App Screenshot Set

Delete an app screenshot set and all of its screenshots.

