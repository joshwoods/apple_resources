

- App Store Connect API
-  List All File Sizes for a Build Bundle 

Web Service Endpoint

# List All File Sizes for a Build Bundle

Get all file sizes for a specific build bundle.

App Store Connect API 1.6+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/buildBundles/{id}/buildBundleFileSizes
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Build Bundles resource.

## Query Parameters

`fields[buildBundleFileSizes]`

`[string]`

Additional fields to include for each Build Bundle File Sizes resource returned by the response.

Possible Values: `deviceModel, osVersion, downloadBytes, installBytes`

`limit`

`integer`

The number of Build Bundle File Sizes resources to return.

Maximum: `200`

## Response Codes

` 200 ``OK`

BuildBundleFileSizesResponse

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

Read App Clip Domain Debug Status Information for a Build Bundle

Get the debug status of the domain you associate with your App Clip for a specific build bundle.

List All Beta App Clip Invocations for a Build Bundle

Get all App Clip invocations you configure for testing for a specific build bundle.

