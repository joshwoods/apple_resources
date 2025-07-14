

- Device Management
-  StatusManagementClientCapabilitiesCapabilities_SupportedPayloadsObject 

Object

# StatusManagementClientCapabilitiesCapabilities_SupportedPayloadsObject

The set of declaration and status items that the client supports.

iOS 15.0+iPadOS 15.0+macOS 13.0+tvOS 16.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object StatusManagementClientCapabilitiesCapabilities_SupportedPayloadsObject
```

## Properties

`declarations`

StatusManagementClientCapabilitiesCapabilities_SupportedPayloads_DeclarationsObject

 (Required) 

A set of declarations that the client supports.

`status-items`

`[string]`

 (Required) 

A list of status items that the client supports.

## See Also

### Supporting Objects

object StatusManagementClientCapabilitiesCapabilitiesObject

A collection of the device’s supported features, payloads, and versions.

object StatusManagementClientCapabilitiesCapabilities_SupportedFeaturesObject

A set of optional protocol features that the client supports.

object StatusManagementClientCapabilitiesCapabilities_SupportedPayloads_DeclarationsObject

A declaration that the client supports.

