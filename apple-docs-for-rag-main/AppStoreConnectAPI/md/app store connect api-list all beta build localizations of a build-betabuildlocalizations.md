

- App Store Connect API
-  List All Beta Build Localizations of a Build 

Web Service Endpoint

# List All Beta Build Localizations of a Build

Get a list of localized beta test information for a specific build.

App Store Connect API 1.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/builds/{id}/betaBuildLocalizations
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource.

## Query Parameters

`fields[betaBuildLocalizations]`

`[string]`

Fields to return for included related types.

Possible Values: `whatsNew, locale, build`

`limit`

`integer`

Number of resources to return.

Maximum: `200`

## Response Codes

` 200 ``OK`

BetaBuildLocalizationsWithoutIncludesResponse

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

### Getting Information Associated with Builds

Read the Build Beta Details Information of a Build

Get the beta test details for a specific build.

Read the App Encryption Declaration of a Build

Read an app encryption declaration associated with a specific build.

Get the App Encryption Declaration ID for a Build

Get the beta app encryption declaration resource ID associated with a build.

