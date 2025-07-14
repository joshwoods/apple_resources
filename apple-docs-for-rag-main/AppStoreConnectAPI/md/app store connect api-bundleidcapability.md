

- App Store Connect API
-  BundleIdCapability 

Object

# BundleIdCapability

The data structure that represents a Bundle ID Capabilities resource.

App Store Connect API 1.1+

``` source
object BundleIdCapability
```

## Properties

`attributes`

BundleIdCapability.Attributes

The resource’s attributes.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the resource.

`links`

ResourceLinks

Navigational links that include the self-link.

`type`

`string`

 (Required) 

The resource type.

Value: `bundleIdCapabilities`

## Topics

### Objects

object BundleIdCapability.Attributes

Attributes that describe a Bundle ID Capabilities resource.

## See Also

### Object and Data Types

object BundleIdCapabilityCreateRequest

The request body you use to create a Bundle ID Capability.

object BundleIdCapabilityUpdateRequest

The request body you use to update a Bundle ID Capability.

object BundleIdCapabilityResponse

A response that contains a single Bundle ID Capabilities resource.

object BundleIdCapabilitiesResponse

A response that contains a list of Bundle ID Capability resources.

object BundleIdCapabilitiesWithoutIncludesResponse

object CapabilityOption

An option within a capability setting.

object CapabilitySetting

An object that represents a capability setting for an app.

type CapabilityType

String that represents an app’s capability type.

