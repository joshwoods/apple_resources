

- Device Management
-  StatusManagementClientCapabilitiesCapabilitiesObject 

Object

# StatusManagementClientCapabilitiesCapabilitiesObject

A collection of the device’s supported features, payloads, and versions.

iOS 15.0+iPadOS 15.0+macOS 13.0+tvOS 16.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object StatusManagementClientCapabilitiesCapabilitiesObject
```

## Properties

`supported-features`

StatusManagementClientCapabilitiesCapabilities_SupportedFeaturesObject

 (Required) 

A set of optional protocol features that the client supports. Each object’s key represents a feature, and the property value represents the feature’s associated parameters.

`supported-payloads`

StatusManagementClientCapabilitiesCapabilities_SupportedPayloadsObject

 (Required) 

A set of declaration and status items that the client supports.

`supported-versions`

`[string]`

 (Required) 

A list of protocol versions that the client supports.

## See Also

### Supporting Objects

object StatusManagementClientCapabilitiesCapabilities_SupportedFeaturesObject

A set of optional protocol features that the client supports.

object StatusManagementClientCapabilitiesCapabilities_SupportedPayloadsObject

The set of declaration and status items that the client supports.

object StatusManagementClientCapabilitiesCapabilities_SupportedPayloads_DeclarationsObject

A declaration that the client supports.

