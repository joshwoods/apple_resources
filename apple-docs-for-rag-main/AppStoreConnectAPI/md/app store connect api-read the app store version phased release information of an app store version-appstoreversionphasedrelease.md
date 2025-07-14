

- App Store Connect API
-  Read the App Store Version Phased Release Information of an App Store Version 

Web Service Endpoint

# Read the App Store Version Phased Release Information of an App Store Version

Read the phased release status and configuration for a version with phased release enabled.

App Store Connect API 1.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appStoreVersions/{id}/appStoreVersionPhasedRelease
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[appStoreVersionPhasedReleases]`

`[string]`

Possible Values: `phasedReleaseState, startDate, totalPauseDuration, currentDayNumber`

## Response Codes

` 200 ``OK`

AppStoreVersionPhasedReleaseWithoutIncludesResponse

`OK`

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

### Reading Release and Review Information

Read the App Store Version Submission Information of an App Store VersionDeprecated

Read the App Store Review Details Resource Information of an App Store Version

Get the details you provide to App Review so they can test your app.

