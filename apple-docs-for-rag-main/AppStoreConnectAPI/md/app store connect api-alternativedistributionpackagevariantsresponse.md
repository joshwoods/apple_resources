

- App Store Connect API
-  AlternativeDistributionPackageVariantsResponse 

Object

# AlternativeDistributionPackageVariantsResponse

A response that contains a list of alternative distribution package variant resources.

App Store Connect API 3.3+

``` source
object AlternativeDistributionPackageVariantsResponse
```

## Properties

`data`

`[`AlternativeDistributionPackageVariant`]`

 (Required) 

`links`

PagedDocumentLinks

 (Required) 

`meta`

PagingInformation

## Discussion

This object is the response that contains a list of alternative distribution package variants. For more information, see List variants information. The schema of the response body is below.

```
{
  "data": [
    {
      "type": "alternativeDistributionPackageVariants",
      "id": "string",
      "attributes": {
        "url": "string",
        "urlExpirationDate": "2024-02-27T00:58:50.105Z",
        "alternativeDistributionKeyBlob": "string"
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

