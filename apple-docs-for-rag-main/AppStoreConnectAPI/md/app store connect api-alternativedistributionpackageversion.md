

- App Store Connect API
-  AlternativeDistributionPackageVersion 

Object

# AlternativeDistributionPackageVersion

The data structure that represents an alternative distribution package version resource.

App Store Connect API 3.3+

``` source
object AlternativeDistributionPackageVersion
```

## Properties

`attributes`

AlternativeDistributionPackageVersion.Attributes

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the alternative distribution package version.

`links`

ResourceLinks

`relationships`

AlternativeDistributionPackageVersion.Relationships

`type`

`string`

 (Required) 

Value: `alternativeDistributionPackageVersions`

## Discussion

For more information about the responses that includes alternative distribution package version objects, see AlternativeDistributionPackageVersionResponse or AlternativeDistributionPackageVersionsResponse.

Tip

Use the `links` fields to navigate the resource object graph while making your requests. For example, from the alternative distribution package version object above, you can also reach its package metadata, deltas, and variants.

## Topics

### Objects

object AlternativeDistributionPackageVersion.Attributes

object AlternativeDistributionPackageVersion.Relationships

## See Also

### Objects

object AlternativeDistributionPackage

The data structure that represents an alternative distribution package resource.

object AlternativeDistributionPackageCreateRequest

The request body you use to create an alternative distribution package.

object AlternativeDistributionPackageResponse

A response that contains a single alternative distribution package resource.

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

