

- App Store Connect API
-  Get the App Store Versions Resource ID for a Default App Clip Experience 

Web Service Endpoint

# Get the App Store Versions Resource ID for a Default App Clip Experience

Get IDs for App Store Versions related to a default App Clip experience.

App Store Connect API 1.6+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appClipDefaultExperiences/{id}/relationships/releaseWithAppStoreVersion
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Default App Clip Experiences resource.

## Response Codes

` 200 ``OK`

AppClipDefaultExperienceReleaseWithAppStoreVersionLinkageResponse

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

### Getting Default App Clip Experience Information

Read Default App Clip Experience Information

Get a specific default App Clip experience.

Read the App Store Review Detail for a Default App Clip Experience

Get App Store Review details for a specific default App Clip experience.

Read Localization Information for a Default App Clip Experience

Get localized metadata that appears on the App Clip card for a specific default App Clip experience.

Read App Store Version Information for a Default App Clip Experience

Get App Store Version information for a default App Clip experience.

