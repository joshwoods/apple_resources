

- App Store Connect API
-  Create a Default App Clip Experience 

Web Service Endpoint

# Create a Default App Clip Experience

Configure a new default App Clip experience.

App Store Connect API 1.6+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/appClipDefaultExperiences
```

## HTTP Body

AppClipDefaultExperienceCreateRequest

The request body you use to create a default App Clip experience.

Content-Type: application/json

## Response Codes

` 201 ``Created`

AppClipDefaultExperienceResponse

`Created`

The request completed successfully and a new default App Clip experience has been created.

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

### Managing Default App Clip Experiences

Modify a Default App Clip Experience

Update a default App Clip experience.

Modify the Related App Store Version for a Default App Clip Experience

Update the relationship between a default App Clip experience and an App Store Version.

Delete a Default App Clip Experience

Delete a specific default App Clip experience.

