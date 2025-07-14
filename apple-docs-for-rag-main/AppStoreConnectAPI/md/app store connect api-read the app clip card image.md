

- App Store Connect API
-  Read the App Clip Card Image 

Web Service Endpoint

# Read the App Clip Card Image

Get the image that appears on the App Clip card of a default App Clip experience.

App Store Connect API 1.6+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appClipHeaderImages/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the App Clip Header Images resource.

## Query Parameters

`fields[appClipHeaderImages]`

`[string]`

Additional fields to include for each App Clip Header Images resource returned by the response.

Possible Values: `fileSize, fileName, sourceFileChecksum, imageAsset, uploadOperations, assetDeliveryState, appClipDefaultExperienceLocalization`

`include`

`[string]`

The relationship data to include in the response.

Value: `appClipDefaultExperienceLocalization`

## Response Codes

` 200 ``OK`

AppClipHeaderImageResponse

`OK`

The request completed successfully.

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

### Managing App Clip Card Images

Create an App Clip Card Image for a Default App Clip Experience

Reserve an image asset that appears on the App Clip card of a default App Clip experience.

Modify an App Clip Card Image

Change the image that appears on the App Clip card of a default App Clip experience.

Delete a Default App Clip Experience Image

Delete the image asset that appears on the App Clip card for a default App Clip experience.

