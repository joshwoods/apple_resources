

- App Store Connect API
-  Read an App Store version’s alternative distribution package 

Web Service Endpoint

# Read an App Store version’s alternative distribution package

Read the alternative distribution package for a specific App Store version.

App Store Connect API 3.3+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appStoreVersions/{id}/alternativeDistributionPackage
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[alternativeDistributionPackageVersions]`

`[string]`

Possible Values: `url, urlExpirationDate, version, fileChecksum, state, variants, deltas, alternativeDistributionPackage`

`fields[alternativeDistributionPackages]`

`[string]`

Value: `versions`

`include`

`[string]`

Value: `versions`

`limit[versions]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

AlternativeDistributionPackageResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Content-Type: application/json

` 404 ``Not Found`

ErrorResponse

`Not Found`

Content-Type: application/json

## Discussion

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/appStoreVersions/f6586f8b-12db-4861-818e-b5cbe0d1736f/alternativeDistributionPackage
```

```
{
  "data": {
    "type": "alternativeDistributionPackages",
    "id": "e651dbc7-a7a7-4e84-a1ae-2afcd92ec6cb",
    "relationships": {
      "versions": {
        "links": {
          "self": "https://api.appstoreconnect.apple.com/v1/alternativeDistributionPackages/e651dbc7-a7a7-4e84-a1ae-2afcd92ec6cb/relationships/versions",
          "related": "https://api.appstoreconnect.apple.com/v1/alternativeDistributionPackages/e651dbc7-a7a7-4e84-a1ae-2afcd92ec6cb/versions"
        }
      }
    },
    "links": {
      "self": "https://api.appstoreconnect.apple.com/v1/alternativeDistributionPackages/e651dbc7-a7a7-4e84-a1ae-2afcd92ec6cb"
    }
  },
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/appStoreVersions/f6586f8b-12db-4861-818e-b5cbe0d1736f/alternativeDistributionPackage"
  }
}
```

## See Also

### Creating and reading distribution packages

Creating alternative distribution packages

Create distribution packages for your apps that you distribute on alternative marketplaces or on the web.

Read alternative distribution package information

Get information about a specific alternative distribution package.

Create an alternative distribution package

Create an alternative distribution package for an app store version.

Read version information for an alternative distribution package

Get version detail information about a specific alternative distribution package.

