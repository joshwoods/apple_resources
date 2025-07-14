

- App Store Connect API
-  Modify and Delete an Advanced App Clip Experience 

Web Service Endpoint

# Modify and Delete an Advanced App Clip Experience

Update and delete an existing advanced App Clip experience.

App Store Connect API 1.6+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/appClipAdvancedExperiences/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Advanced App Clip Experiences resource.

## HTTP Body

AppClipAdvancedExperienceUpdateRequest

The request body you use to update an advanced App Clip experience.

Content-Type: application/json

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

The provided resource data is not valid.

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## See Also

### Getting and Managing Advanced App Clip Experiences

Read Advanced App Clip Experience Information

Get information about a specific advanced App Clip experience.

Create an Advanced App Clip Experience

Configure a new advanced App Clip experience.

