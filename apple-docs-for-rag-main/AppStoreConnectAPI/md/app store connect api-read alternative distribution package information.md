

- App Store Connect API
-  Read alternative distribution package information 

Web Service Endpoint

# Read alternative distribution package information

Get information about a specific alternative distribution package.

App Store Connect API 3.3+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/alternativeDistributionPackages/{id}
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
https://api.appstoreconnect.apple.com/v1/alternativeDistributionPackages/c925443b-7dfb-4cc5-8b1a-0074eb7d5fe9
```

```

{
  "data" : {
    "type" : "alternativeDistributionPackages",
    "id" : "c925443b-7dfb-4cc5-8b1a-0074eb7d5fe9",
    "relationships" : {
      "versions" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/alternativeDistributionPackages/c925443b-7dfb-4cc5-8b1a-0074eb7d5fe9/relationships/versions",
          "related" : "https://api.appstoreconnect.apple.com/v1/alternativeDistributionPackages/c925443b-7dfb-4cc5-8b1a-0074eb7d5fe9/versions"
        }
      }
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v1/alternativeDistributionPackages/c925443b-7dfb-4cc5-8b1a-0074eb7d5fe9"
    }
  },
  "links" : {
    "self" : "https://api.appstoreconnect.apple.com/v1/alternativeDistributionPackages/c925443b-7dfb-4cc5-8b1a-0074eb7d5fe9"
  }
}
```

## See Also

### Creating and reading distribution packages

Creating alternative distribution packages

Create distribution packages for your apps that you distribute on alternative marketplaces or on the web.

Create an alternative distribution package

Create an alternative distribution package for an app store version.

Read an App Store version’s alternative distribution package

Read the alternative distribution package for a specific App Store version.

Read version information for an alternative distribution package

Get version detail information about a specific alternative distribution package.

