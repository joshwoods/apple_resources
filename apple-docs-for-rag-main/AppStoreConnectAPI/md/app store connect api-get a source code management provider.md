

- App Store Connect API
-  Get a Source Code Management Provider 

Web Service Endpoint

# Get a Source Code Management Provider

Get information about a specific source code management provider you connected to Xcode Cloud.

App Store Connect API 1.5+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/scmProviders/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Providers resource.

## Query Parameters

`fields[scmProviders]`

`[string]`

Additional fields to include for the Providers resource returned by the response.

Possible Values: `scmProviderType, url, repositories`

## Response Codes

` 200 ``OK`

ScmProviderResponse

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

## Discussion

The example request below retrieves information about a specific source code management provider you connected to Xcode Cloud. Use the data provided in the response to read additional information; for example, repository information.

### Example Request and Response

- Request
- Response

```
GET https://api.appstoreconnect.apple.com/v1/scmProviders/d1b5479e-ce72-402c-8b9a-ea26ef6773f4
```

```
{
    "data": {
        "type": "scmProviders",
        "id": "d1b5479e-ce72-402c-8b9a-ea26ef6773f4",
        "attributes": {
            "scmProviderType": {
                "kind": "GITHUB_CLOUD",
                "displayName": "GitHub",
                "isOnPremise": false
            },
            "url": "github.com"
        },
        "relationships": {
            "repositories": {
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/scmProviders/d1b5479e-ce72-402c-8b9a-ea26ef6773f4/relationships/repositories",
                    "related": "https://api.appstoreconnect.apple.com/v1/scmProviders/d1b5479e-ce72-402c-8b9a-ea26ef6773f4/repositories"
                }
            }
        },
        "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/scmProviders/d1b5479e-ce72-402c-8b9a-ea26ef6773f4"
        }
    },
    "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/scmProviders/d1b5479e-ce72-402c-8b9a-ea26ef6773f4"
    }
}
```

## See Also

### Getting Provider Information

List All Source Code Management Providers

List all source code management providers you connected to Xcode Cloud.

List all Repositories for a Source Code Management Provider

List all Git repositories for a specific source code management provider you connected to Xcode Cloud.

