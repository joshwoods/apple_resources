

- App Store Connect API
-  BundleId 

Object

# BundleId

The data structure that represents a Bundle IDs resource.

App Store Connect API 1.1+

``` source
object BundleId
```

## Properties

`attributes`

BundleId.Attributes

The resource’s attributes.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the resource.

`relationships`

BundleId.Relationships

Navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `bundleIds`

`links`

ResourceLinks

Navigational links that include the self-link.

## Topics

### Objects

object BundleId.Attributes

Attributes that describe a Bundle IDs resource.

object BundleId.Relationships

The relationships you included in the request and those on which you can operate.

## See Also

### Objects and Types

type BundleIdPlatform

Strings that represent the operating system intended for the bundle.

object BundleIdCreateRequest

The request body you use to create a Bundle ID.

object BundleIdUpdateRequest

The request body you use to update a Bundle ID.

object BundleIdResponse

A response that contains a single Bundle IDs resource.

object BundleIdWithoutIncludesResponse

object BundleIdsResponse

A response that contains a list of Bundle ID resources.

