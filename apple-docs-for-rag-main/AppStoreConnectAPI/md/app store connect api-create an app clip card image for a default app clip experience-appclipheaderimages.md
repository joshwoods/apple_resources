

- App Store Connect API
-  Create an App Clip Card Image for a Default App Clip Experience 

Web Service Endpoint

# Create an App Clip Card Image for a Default App Clip Experience

Reserve an image asset that appears on the App Clip card of a default App Clip experience.

App Store Connect API 1.6+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/appClipHeaderImages
```

## HTTP Body

AppClipHeaderImageCreateRequest

The request body you use to create an App Clip header image.

Content-Type: application/json

## Response Codes

` 201 ``Created`

AppClipHeaderImageResponse

`Created`

The request completed successfully and a new App Clip Header Images resource has been created.

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

### Managing App Clip Card Images

Read the App Clip Card Image

Get the image that appears on the App Clip card of a default App Clip experience.

Modify an App Clip Card Image

Change the image that appears on the App Clip card of a default App Clip experience.

Delete a Default App Clip Experience Image

Delete the image asset that appears on the App Clip card for a default App Clip experience.

