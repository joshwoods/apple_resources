

- App Store Connect API
-  AlternativeDistributionPackageDelta 

Object

# AlternativeDistributionPackageDelta

The data structure that represents an alternative distribution package delta resource.

App Store Connect API 3.3+

``` source
object AlternativeDistributionPackageDelta
```

## Properties

`attributes`

AlternativeDistributionPackageDelta.Attributes

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the alternative distribution package delta.

`links`

ResourceLinks

`type`

`string`

 (Required) 

Value: `alternativeDistributionPackageDeltas`

## Discussion

For more information about the responses that include alternative distribution package delta objects, see AlternativeDistributionPackageDeltaResponse or AlternativeDistributionPackageDeltasResponse.

Tip

Use the `links` fields to navigate the resource object graph while making your requests. For example, from the alternative distribution package delta object above, you can also reach its package metadata, versions, and variants.

## Topics

### Objects

object AlternativeDistributionPackageDelta.Attributes

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

