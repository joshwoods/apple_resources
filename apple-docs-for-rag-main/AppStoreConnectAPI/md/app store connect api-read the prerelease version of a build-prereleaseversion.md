

- App Store Connect API
-  Read the Prerelease Version of a Build 

Web Service Endpoint

# Read the Prerelease Version of a Build

Get the prerelease version for a specific build.

App Store Connect API 1.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/builds/{id}/preReleaseVersion
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource.

## Query Parameters

`fields[preReleaseVersions]`

`[string]`

Fields to return for included related types.

Possible Values: `version, platform, builds, app`

## Response Codes

` 200 ``OK`

PrereleaseVersionWithoutIncludesResponse

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

### Getting Build Information

List Builds

Find and list builds for all apps in App Store Connect.

Read Build Information

Get information about a specific build.

Read the App Information of a Build

Get the app information for a specific build.

Read the App Store Version Information of a Build

Get the App Store version of a specific build.

Read usage metrics for a beta build

Get usage metrics for a specific build.

