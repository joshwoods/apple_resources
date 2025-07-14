

- Enterprise Program API
-  CapabilitySetting 

Object

# CapabilitySetting

An object that represents a capability setting for an app.

``` source
object CapabilitySetting
```

## Properties

`allowedInstances`

`string`

Possible Values: `ENTRY, SINGLE, MULTIPLE`

`description`

`string`

`enabledByDefault`

`boolean`

`key`

`string`

Possible Values: `ICLOUD_VERSION, DATA_PROTECTION_PERMISSION_LEVEL, APPLE_ID_AUTH_APP_CONSENT`

`minInstances`

`integer`

`name`

`string`

`options`

`[`CapabilityOption`]`

`visible`

`boolean`

## Attributes 

Possible types:

## See Also

### Object and Data Types

object BundleIdCapability

The data structure that represents a Bundle ID Capabilities resource.

object BundleIdCapabilityCreateRequest

The request body you use to create a Bundle ID Capability.

object BundleIdCapabilityUpdateRequest

The request body you use to update a Bundle ID Capability.

object BundleIdCapabilityResponse

A response that contains a single Bundle ID Capabilities resource.

object BundleIdCapabilitiesResponse

A response that contains a list of Bundle ID Capability resources.

object BundleIdCapabilitiesWithoutIncludesResponse

A response that contains a single Bundle IDs capability resource without includes.

object CapabilityOption

An option within a capability setting.

type CapabilityType

String that represents an app’s capability type.

