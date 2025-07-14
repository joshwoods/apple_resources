

- Enterprise Program API
-  BundleIdCapabilitiesResponse 

Object

# BundleIdCapabilitiesResponse

A response that contains a list of Bundle ID Capability resources.

``` source
object BundleIdCapabilitiesResponse
```

## Properties

`data`

`[`BundleIdCapability`]`

 (Required) 

The resource data.

`links`

PagedDocumentLinks

 (Required) 

Navigational links that include the self-link.

`meta`

PagingInformation

Paging information.

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

object BundleIdCapabilitiesWithoutIncludesResponse

A response that contains a single Bundle IDs capability resource without includes.

object CapabilityOption

An option within a capability setting.

object CapabilitySetting

An object that represents a capability setting for an app.

type CapabilityType

String that represents an app’s capability type.

