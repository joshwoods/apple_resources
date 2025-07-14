

- App Store Connect API
-  List All Source Code Management Providers 

Web Service Endpoint

# List All Source Code Management Providers

List all source code management providers you connected to Xcode Cloud.

App Store Connect API 1.5+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/scmProviders
```

## Query Parameters

`fields[scmProviders]`

`[string]`

Additional fields to include for each Providers resource returned by the response.

Possible Values: `scmProviderType, url, repositories`

`limit`

`integer`

The number of Providers resources to return.

Maximum: `200`

## Response Codes

` 200 ``OK`

ScmProvidersResponse

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

## See Also

### Getting Provider Information

Get a Source Code Management Provider

Get information about a specific source code management provider you connected to Xcode Cloud.

List all Repositories for a Source Code Management Provider

List all Git repositories for a specific source code management provider you connected to Xcode Cloud.

