

- App Store Connect API
-  AlternativeDistributionPackageVariant 

Object

# AlternativeDistributionPackageVariant

The data structure that represents an alternative distribution package variant resource.

App Store Connect API 3.3+

``` source
object AlternativeDistributionPackageVariant
```

## Properties

`attributes`

AlternativeDistributionPackageVariant.Attributes

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the alternative distribution package variant.

`links`

ResourceLinks

`type`

`string`

 (Required) 

Value: `alternativeDistributionPackageVariants`

## Discussion

To learn more about the responses that include alternative distribution package variant objects, see AlternativeDistributionPackageVariantResponse or AlternativeDistributionPackageVariantsResponse.

Tip

Use the `links` fields to navigate the resource object graph while making your requests. For example, from the alternative distribution package variant object above, you can also reach its package metadata, deltas, and versions.

## Topics

### Objects

object AlternativeDistributionPackageVariant.Attributes

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

object AlternativeDistributionPackageVariantResponse

A response that contains a single alternative distribution package variant resource.

object AlternativeDistributionPackageVariantsResponse

A response that contains a list of alternative distribution package variant resources.

