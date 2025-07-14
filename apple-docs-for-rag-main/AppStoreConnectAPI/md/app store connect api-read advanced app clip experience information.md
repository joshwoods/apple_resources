

- App Store Connect API
-  Read Advanced App Clip Experience Information 

Web Service Endpoint

# Read Advanced App Clip Experience Information

Get information about a specific advanced App Clip experience.

App Store Connect API 1.6+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appClipAdvancedExperiences/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Advanced App Clip Experiences resource.

## Query Parameters

`fields[appClipAdvancedExperiences]`

`[string]`

Additional fields to include for each Advanced App Clip Experiences resource returned by the response.

Possible Values: `link, version, status, action, isPoweredBy, place, placeStatus, businessCategory, defaultLanguage, appClip, headerImage, localizations`

`include`

`[string]`

The relationship data to include in the response.

Possible Values: `appClip, headerImage, localizations`

`limit[localizations]`

`integer`

The number of included Advanced App Clip Experiences resources to return if the advanced App Clip experience localizations relationship is included.

Maximum: `50`

## Response Codes

` 200 ``OK`

AppClipAdvancedExperienceResponse

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

### Getting and Managing Advanced App Clip Experiences

Create an Advanced App Clip Experience

Configure a new advanced App Clip experience.

Modify and Delete an Advanced App Clip Experience

Update and delete an existing advanced App Clip experience.

