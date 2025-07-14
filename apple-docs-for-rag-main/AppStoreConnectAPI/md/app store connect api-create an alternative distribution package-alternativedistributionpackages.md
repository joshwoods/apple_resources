

- App Store Connect API
-  Create an alternative distribution package 

Web Service Endpoint

# Create an alternative distribution package

Create an alternative distribution package for an app store version.

App Store Connect API 3.3+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/alternativeDistributionPackages
```

## HTTP Body

AlternativeDistributionPackageCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

AlternativeDistributionPackageResponse

`Created`

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## Mentioned in 

Creating alternative distribution packages

Configuring apps for web distribution

Configuring alternative marketplaces and alternative marketplace apps

## Discussion

Tip

This endpoint requires the `appStoreVersion` in the payload. Obtain the `appStoreVersion` resource ID from the List All App Store Versions for an App response.

### Example Request and Response

- Request
- Response

```
POST https://api.appstoreconnect.apple.com/v1/alternativeDistributionPackages
{
  "data": {
    "type": "alternativeDistributionPackages",
    "relationships": {
      "appStoreVersion": {
        "data": {
          "type": "appStoreVersions",
          "id": "3fb74833-4bf4-4c34-9cfd-f9dc4978ea45"
        }
      }
    }
  }
}
```

```
{
  "data": {
    "type": "alternativeDistributionPackages",
    "id": "f3190601-974c-45ee-aa24-35db2090c260",
    "relationships": {
      "versions": {
        "links": {
          "self": "https://api.appstoreconnect.apple.com/v1/alternativeDistributionPackages/f3190601-974c-45ee-aa24-35db2090c260/relationships/versions",
          "related": "https://api.appstoreconnect.apple.com/v1/alternativeDistributionPackages/f3190601-974c-45ee-aa24-35db2090c260/versions"
        }
      }
    },
    "links": {
      "self": "https://api.appstoreconnect.apple.com/v1/alternativeDistributionPackages/f3190601-974c-45ee-aa24-35db2090c260"
    }
  },
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/alternativeDistributionPackages"
  }
}
```

## See Also

### Creating and reading distribution packages

Creating alternative distribution packages

Create distribution packages for your apps that you distribute on alternative marketplaces or on the web.

Read alternative distribution package information

Get information about a specific alternative distribution package.

Read an App Store version’s alternative distribution package

Read the alternative distribution package for a specific App Store version.

Read version information for an alternative distribution package

Get version detail information about a specific alternative distribution package.

