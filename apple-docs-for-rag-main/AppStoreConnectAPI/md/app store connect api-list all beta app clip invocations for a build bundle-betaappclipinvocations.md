

- App Store Connect API
-  List All Beta App Clip Invocations for a Build Bundle 

Web Service Endpoint

# List All Beta App Clip Invocations for a Build Bundle

Get all App Clip invocations you configure for testing for a specific build bundle.

App Store Connect API 1.6+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/buildBundles/{id}/betaAppClipInvocations
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Build Bundles resource.

## Query Parameters

`fields[betaAppClipInvocationLocalizations]`

`[string]`

Additional fields to include for each Beta App Clip Invocation resource returned by the response.

Possible Values: `title, locale`

`fields[betaAppClipInvocations]`

`[string]`

Additional fields to include for each Beta App Clip Invocation resource returned by the response.

Possible Values: `url, betaAppClipInvocationLocalizations`

`include`

`[string]`

The relationship data to include in the response.

Value: `betaAppClipInvocationLocalizations`

`limit`

`integer`

The number of Beta App Clip Invocations resources to return.

Maximum: `200`

`limit[betaAppClipInvocationLocalizations]`

`integer`

The number of included Beta App Clip Invocations resources to return if the beta App Clip invocation localizations relationship is included.

Maximum: `50`

## Response Codes

` 200 ``OK`

BetaAppClipInvocationsResponse

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

List All File Sizes for a Build Bundle

Get all file sizes for a specific build bundle.

