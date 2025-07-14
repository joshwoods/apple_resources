

- Device Management
-  StatusManagementClientCapabilitiesCapabilities_SupportedPayloads_DeclarationsObject 

Object

# StatusManagementClientCapabilitiesCapabilities_SupportedPayloads_DeclarationsObject

A declaration that the client supports.

iOS 15.0+iPadOS 15.0+macOS 13.0+tvOS 16.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object StatusManagementClientCapabilitiesCapabilities_SupportedPayloads_DeclarationsObject
```

## Properties

`activations`

`[string]`

An array of strings that represents the activation types that the client supports.

`assets`

`[string]`

An array of strings that represents the assets that the client supports.

`configurations`

`[string]`

An array of strings that represents the configuration types that the client supports.

`management`

`[string]`

An array of strings that represents the declaration types that the client supports.

## See Also

### Supporting Objects

object StatusManagementClientCapabilitiesCapabilitiesObject

A collection of the device’s supported features, payloads, and versions.

object StatusManagementClientCapabilitiesCapabilities_SupportedFeaturesObject

A set of optional protocol features that the client supports.

object StatusManagementClientCapabilitiesCapabilities_SupportedPayloadsObject

The set of declaration and status items that the client supports.

