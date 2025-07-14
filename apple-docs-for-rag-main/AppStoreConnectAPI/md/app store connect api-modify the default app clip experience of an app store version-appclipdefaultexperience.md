

- App Store Connect API
-  Modify the Default App Clip Experience of an App Store Version 

Web Service Endpoint

# Modify the Default App Clip Experience of an App Store Version

Update the relationship between an App Store version and a default App Clip experience.

App Store Connect API 1.6+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/appStoreVersions/{id}/relationships/appClipDefaultExperience
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the App Store Versions resource.

## HTTP Body

AppStoreVersionAppClipDefaultExperienceLinkageRequest

The request body you use to update the relationship between an App Store version and a default App Clip experience.

Content-Type: application/json

## Response Codes

` 204 ``No Content`

`No Content`

The request completed successfully and the relationship with the specific default App Clip experience was updated.

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

### Attaching a Default App Clip Experience to a Version

Get the Default App Clip Experience for an App Store Version

Get the default App Clip experience for an App Store version of your app.

Get the Default App Clip Experiences Resource ID for an App Store Version

Get the ID of an app’s related default App Clip experience.

