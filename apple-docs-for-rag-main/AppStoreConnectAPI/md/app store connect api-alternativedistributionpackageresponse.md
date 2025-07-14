

- App Store Connect API
-  AlternativeDistributionPackageResponse 

Object

# AlternativeDistributionPackageResponse

A response that contains a single alternative distribution package resource.

App Store Connect API 3.3+

``` source
object AlternativeDistributionPackageResponse
```

## Properties

`data`

AlternativeDistributionPackage

 (Required) 

`included`

`[`AlternativeDistributionPackageVersion`]`

`links`

DocumentLinks

 (Required) 

## Discussion

This object is the response that contains a single the alternative distribution package. For more information, see Creating and reading distribution packages. The schema of the response body is below.

```
{
  "data": {
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
  },
  "included": [
    {
      "type": "alternativeDistributionPackageVersions",
      "id": "string",
      "attributes": {
        "url": "string",
        "urlExpirationDate": "2024-02-23T15:32:57.654Z",
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
    }
  ],
  "links": {
    "self": "string"
  }
}
```

## See Also

### Objects

object AlternativeDistributionPackage

The data structure that represents an alternative distribution package resource.

object AlternativeDistributionPackageCreateRequest

The request body you use to create an alternative distribution package.

object AlternativeDistributionPackageVersion

The data structure that represents an alternative distribution package version resource.

object AlternativeDistributionPackageVersionResponse

A response that contains a single alternative distribution package version resource.

object AlternativeDistributionPackageVersionsResponse

A response that contains a list of alternative distribution package version resources.

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

