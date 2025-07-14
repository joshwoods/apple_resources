

- App Store Connect API
-  AlternativeDistributionPackageVariantResponse 

Object

# AlternativeDistributionPackageVariantResponse

A response that contains a single alternative distribution package variant resource.

App Store Connect API 3.3+

``` source
object AlternativeDistributionPackageVariantResponse
```

## Properties

`data`

AlternativeDistributionPackageVariant

 (Required) 

`links`

DocumentLinks

 (Required) 

## Discussion

This object is the response that contains a single alternative distribution package variant. For more information, see Read information for an alternative distribution package variants. The schema of the response body is below.

```
{
  "data": {
    "type": "alternativeDistributionPackageVariants",
    "id": "string",
    "attributes": {
      "url": "string",
      "urlExpirationDate": "2025-02-23T06:53:07.520Z",
      "alternativeDistributionKeyBlob": "string"
    },
    "links": {
      "self": "string"
    }
  },
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

object AlternativeDistributionPackageVariantsResponse

A response that contains a list of alternative distribution package variant resources.

