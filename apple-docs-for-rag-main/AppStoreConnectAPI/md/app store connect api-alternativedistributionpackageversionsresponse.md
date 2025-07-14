

- App Store Connect API
-  AlternativeDistributionPackageVersionsResponse 

Object

# AlternativeDistributionPackageVersionsResponse

A response that contains a list of alternative distribution package version resources.

App Store Connect API 3.3+

``` source
object AlternativeDistributionPackageVersionsResponse
```

## Properties

`data`

`[`AlternativeDistributionPackageVersion`]`

 (Required) 

`included`

`[*]`

Possible types: AlternativeDistributionPackageVariant`, `AlternativeDistributionPackageDelta`, `AlternativeDistributionPackage

`links`

PagedDocumentLinks

 (Required) 

`meta`

PagingInformation

## Discussion

This object is the response that contains a list of alternative distribution package versions. For more information, see Read version information for an alternative distribution package. The schema of the response body is below.

```
{
  "data": [
    {
      "type": "alternativeDistributionPackageVersions",
      "id": "string",
      "attributes": {
        "url": "string",
        "urlExpirationDate": "2025-02-23T06:55:44.288Z",
        "version": "string",
        "state": "COMPLETED"
      },
      "relationships": {
        "variants": {
          "links": {
            "self": "string",
            "related": "string"
          },
          "meta": {
            "paging": {
              "total": 0,
              "limit": 0
            }
          },
          "data": [
            {
              "type": "alternativeDistributionPackageVariants",
              "id": "string"
            }
          ]
        },
        "deltas": {
          "links": {
            "self": "string",
            "related": "string"
          },
          "meta": {
            "paging": {
              "total": 0,
              "limit": 0
            }
          },
          "data": [
            {
              "type": "alternativeDistributionPackageDeltas",
              "id": "string"
            }
          ]
        },
        "alternativeDistributionPackage": {
          "links": {
            "self": "string",
            "related": "string"
          },
          "data": {
            "type": "alternativeDistributionPackages",
            "id": "string"
          }
        }
      },
      "links": {
        "self": "string"
      }
    },
    "included": [
      {
        "type": "alternativeDistributionPackageVariants",
        "id": "string",
        "attributes": {
          "url": "string",
          "urlExpirationDate": "2025-02-23T06:55:44.288Z",
          "alternativeDistributionKeyBlob": "string"
        },
        "links": {
          "self": "string"
        }
      },
      {
        "type": "alternativeDistributionPackageDeltas",
        "id": "string",
        "attributes": {
          "url": "string",
          "urlExpirationDate": "2025-02-23T06:55:44.288Z",
          "alternativeDistributionKeyBlob": "string"
        },
        "links": {
          "self": "string"
        }
      },
      {
        "type": "alternativeDistributionPackages",
        "id": "string",
          "relationships": {
          "versions": {
            "links": {
              "self": "string",
              "related": "string"
            },
            "meta": {
              "paging": {
                "total": 0,
                "limit": 0
              }
            },
            "data": [
              {
                "type": "alternativeDistributionPackageVersions",
                "id": "string"
              }
            ]
          }
        },
        "links": {
          "self": "string"
        }
      }
    ],
    "links": {
      "self": "string",
      "first": "string",
      "next": "string"
    },
    "meta": {
      "paging": {
        "total": 0,
        "limit": 0
      }
    }
  }
}
```

## See Also

### Objects

object AlternativeDistributionPackage

The data structure that represents an alternative distribution package resource.

object AlternativeDistributionPackageCreateRequest

The request body you use to create an alternative distribution package.

object AlternativeDistributionPackageResponse

A response that contains a single alternative distribution package resource.

object AlternativeDistributionPackageVersion

The data structure that represents an alternative distribution package version resource.

object AlternativeDistributionPackageVersionResponse

A response that contains a single alternative distribution package version resource.

object AlternativeDistributionPackageDelta

The data structure that represents an alternative distribution package delta resource.

object AlternativeDistributionPackageDeltaResponse

A response that contains a single alternative distribution package delta resource.

object AlternativeDistributionPackageDeltasResponse

A response that contains a list of alternative distribution package delta resources.

object AlternativeDistributionPackageVariant

The data structure that represents an alternative distribution package variant resource.

object AlternativeDistributionPackageVariantResponse

A response that contains a single alternative distribution package variant resource.

object AlternativeDistributionPackageVariantsResponse

A response that contains a list of alternative distribution package variant resources.

