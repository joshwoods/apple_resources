

- App Store Connect API
-  Read App Clip Domain Debug Status Information for a Build Bundle 

Web Service Endpoint

# Read App Clip Domain Debug Status Information for a Build Bundle

Get the debug status of the domain you associate with your App Clip for a specific build bundle.

App Store Connect API 1.6+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/buildBundles/{id}/appClipDomainDebugStatus
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Build Bundles resource.

## Query Parameters

`fields[appClipDomainStatuses]`

`[string]`

Additional fields to include for each App Clip Domain Debug Statuses resource returned by the response.

Possible Values: `domains, lastUpdatedDate`

## Response Codes

` 200 ``OK`

AppClipDomainStatusResponse

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

### Getting Build Bundle Information

Read the App Clip Domain Cache Status Information for a Build Bundle

Get the cache status of the domain you associate with your App Clip for a specific build bundle.

List All Beta App Clip Invocations for a Build Bundle

Get all App Clip invocations you configure for testing for a specific build bundle.

List All File Sizes for a Build Bundle

Get all file sizes for a specific build bundle.

