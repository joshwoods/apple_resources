

- App Store Connect API
-  Create an Advanced App Clip Experience 

Web Service Endpoint

# Create an Advanced App Clip Experience

Configure a new advanced App Clip experience.

App Store Connect API 1.6+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/appClipAdvancedExperiences
```

## HTTP Body

AppClipAdvancedExperienceCreateRequest

The request body you use to create a new advanced App Clip experience.

Content-Type: application/json

## Response Codes

` 201 ``Created`

AppClipAdvancedExperienceResponse

`Created`

The request completed successfully and a new advanced App Clip experience has been created.

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

### Getting and Managing Advanced App Clip Experiences

Read Advanced App Clip Experience Information

Get information about a specific advanced App Clip experience.

Modify and Delete an Advanced App Clip Experience

Update and delete an existing advanced App Clip experience.

