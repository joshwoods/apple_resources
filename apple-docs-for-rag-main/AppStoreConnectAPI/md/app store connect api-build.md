

- App Store Connect API
-  Build 

Object

# Build

The data structure that represents a Builds resource.

App Store Connect API 1.0+

``` source
object Build
```

## Properties

`attributes`

Build.Attributes

The resource’s attributes.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the resource.

`relationships`

Build.Relationships

Navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `builds`

`links`

ResourceLinks

Navigational links that include the self-link.

## Topics

### Attributes and Relationships

object Build.Attributes

Attributes that describe a Builds resource.

object Build.Relationships

The relationships you included in the request and those on which you can operate.

## See Also

### Objects

object BuildResponse

A response that contains a single Builds resource.

object BuildWithoutIncludesResponse

object BuildsResponse

A response that contains a list of Builds resources.

object BuildsWithoutIncludesResponse

object BuildUpdateRequest

The request body you use to update a Build.

object BuildAppEncryptionDeclarationLinkageRequest

The request body you use to attach an app encryption declaration to a build.

object BuildAppEncryptionDeclarationLinkageResponse

A response body that contains the ID of a single related resource.

object BuildIndividualTestersLinkagesRequest

A request body you use to add or remove a build from multiple beta groups.

object BuildIndividualTestersLinkagesResponse

A response body that contains a list of related resource IDs.

object BuildBetaGroupsLinkagesRequest

A request body you use to add or remove beta groups from a build.

object ImageAsset

An image asset, including its height, width, and template URL.

object BetaBuildUsagesV1MetricResponse

A response that contains one or more beta build metric resources.

