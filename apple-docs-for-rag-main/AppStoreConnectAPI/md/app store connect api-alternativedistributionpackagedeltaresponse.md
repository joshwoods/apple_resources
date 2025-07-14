

- App Store Connect API
-  AlternativeDistributionPackageDeltaResponse 

Object

# AlternativeDistributionPackageDeltaResponse

A response that contains a single alternative distribution package delta resource.

App Store Connect API 3.3+

``` source
object AlternativeDistributionPackageDeltaResponse
```

## Properties

`data`

AlternativeDistributionPackageDelta

 (Required) 

`links`

DocumentLinks

 (Required) 

## Discussion

This object is the response that contains a single alternative distribution package delta. For more information about alternative distribution package deltas see Read information for alternative distribution package deltas. The schema of the response body is below.

```
{
  "data": {
    "type": "alternativeDistributionPackageDeltas",
    "id": "string",
    "attributes": {
      "url": "string",
      "urlExpirationDate": "2024-02-23T06:50:07.723Z",
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

object AlternativeDistributionPackageDeltasResponse

A response that contains a list of alternative distribution package delta resources.

object AlternativeDistributionPackageVariant

The data structure that represents an alternative distribution package variant resource.

object AlternativeDistributionPackageVariantResponse

A response that contains a single alternative distribution package variant resource.

object AlternativeDistributionPackageVariantsResponse

A response that contains a list of alternative distribution package variant resources.

