

- App Store Connect API
-  Modify a Default App Clip Experience 

Web Service Endpoint

# Modify a Default App Clip Experience

Update a default App Clip experience.

App Store Connect API 1.6+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/appClipDefaultExperiences/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Default App Clip Experiences resource.

## HTTP Body

AppClipDefaultExperienceUpdateRequest

The request body you use to update a default App Clip experience.

Content-Type: application/json

## Response Codes

` 200 ``OK`

AppClipDefaultExperienceResponse

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

### Managing Default App Clip Experiences

Create a Default App Clip Experience

Configure a new default App Clip experience.

Modify the Related App Store Version for a Default App Clip Experience

Update the relationship between a default App Clip experience and an App Store Version.

Delete a Default App Clip Experience

Delete a specific default App Clip experience.

