

- App Store Connect API
-  Read information for an alternative distribution package version 

Web Service Endpoint

# Read information for an alternative distribution package version

Get detail information about a specific alternative distribution package version.

App Store Connect API 3.3+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/alternativeDistributionPackageVersions/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[alternativeDistributionPackageDeltas]`

`[string]`

Possible Values: `url, urlExpirationDate, alternativeDistributionKeyBlob, fileChecksum`

`fields[alternativeDistributionPackageVariants]`

`[string]`

Possible Values: `url, urlExpirationDate, alternativeDistributionKeyBlob, fileChecksum`

`fields[alternativeDistributionPackageVersions]`

`[string]`

Possible Values: `url, urlExpirationDate, version, fileChecksum, state, variants, deltas, alternativeDistributionPackage`

`include`

`[string]`

Possible Values: `variants, deltas, alternativeDistributionPackage`

`limit[deltas]`

`integer`

Maximum: `50`

`limit[variants]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

AlternativeDistributionPackageVersionResponse

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
https://api.appstoreconnect.apple.com/v1/alternativeDistributionPackageVersions/d1663e24-4360-4f7f-a661-8e616e3b3c3b
```

```
{
  "data": {
    "type": "alternativeDistributionPackageVersions",
    "id": "d1663e24-4360-4f7f-a661-8e616e3b3c3b",
    "attributes": {
      "url": "https://iosapps.itunes.apple.com/itunes-assets/SWDistributionArtifacts123/v4/0f/8a/35/0f8a3516-32b0-2f72-86be-733c19d4feea/alternative-distribution-package.zip?accessKey=1711772539_4058138271381390069_MNqOb5cg54HQ8yX%2B%2B2Vdqr2zloVZc%2FhvKpOKC2aMcu2ktV%2BhmRoZquZJg%2BHbxrjbnRRSoqNuLQ07Y59co1q4YT2k8ikLRfUL8ZOjB6SZ4s4W3hfIquIZ6WQNoGHQ4YUwb1xVqAkNzgjgVVjp6Z41Cvuw0dyWtAQr9eJ1Q2tRd%2F5soBjsEiWWmkGI%2BZx2ByMkj5qlk9HXY%2BIkoU2XC9kQO6RyTR1YHv1JdHrw%2FNRj%2FvY%3D",
      "urlExpirationDate": "2024-03-29T21:22:19-07:00",
      "version": "1",
      "state": "COMPLETED"
    },
    "relationships": {
      "variants": {
        "links": {
          "self": "https://api.appstoreconnect.apple.com/v1/alternativeDistributionPackageVersions/d1663e24-4360-4f7f-a661-8e616e3b3c3b/relationships/variants",
          "related": "https://api.appstoreconnect.apple.com/v1/alternativeDistributionPackageVersions/d1663e24-4360-4f7f-a661-8e616e3b3c3b/variants"
        }
      },
      "deltas": {
        "links": {
          "self": "https://api.appstoreconnect.apple.com/v1/alternativeDistributionPackageVersions/d1663e24-4360-4f7f-a661-8e616e3b3c3b/relationships/deltas",
          "related": "https://api.appstoreconnect.apple.com/v1/alternativeDistributionPackageVersions/d1663e24-4360-4f7f-a661-8e616e3b3c3b/deltas"
        }
      }
    },
    "links": {
      "self": "https://api.appstoreconnect.apple.com/v1/alternativeDistributionPackageVersions/d1663e24-4360-4f7f-a661-8e616e3b3c3b"
    }
  },
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/alternativeDistributionPackageVersions/d1663e24-4360-4f7f-a661-8e616e3b3c3b"
  }
}

```

## See Also

### Getting version information

Read version information for an alternative distribution package

Get version detail information about a specific alternative distribution package.

List deltas information

List deltas for a specific alternative distribution package version.

List variants information

List variants for specific alternative distribution package version.

