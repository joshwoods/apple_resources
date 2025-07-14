

- App Store Connect API
-  Modify the Image for an Advanced App Clip Experience 

Web Service Endpoint

# Modify the Image for an Advanced App Clip Experience

Update image information or commit the image asset of an advanced App Clip experience.

App Store Connect API 1.6+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/appClipAdvancedExperienceImages/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Advanced App Clip Experience Images resource.

## HTTP Body

AppClipAdvancedExperienceImageUpdateRequest

The request body you use to update the image asset for an advanced App Clip experience.

Content-Type: application/json

## Response Codes

` 200 ``OK`

AppClipAdvancedExperienceImageResponse

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

The provided resource data is not valid.

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## See Also

### Managing Images for Advanced App Clip Experiences

Read Image Information for an Advanced App Clip Experience

Get information about the image that appears on the App Clip card of an advanced App Clip experience.

Create an App Clip Card Image for an Advanced App Clip Experience

Reserve an image asset that appears on the App Clip card of an advanced App Clip experience.

