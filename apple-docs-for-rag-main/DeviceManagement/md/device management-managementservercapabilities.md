

- Device Management
-  ManagementServerCapabilities 

Object

# ManagementServerCapabilities

The declaration to configure the server’s feature set.

iOS 15.0+iPadOS 15.0+macOS 13.0+tvOS 16.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object ManagementServerCapabilities
```

## Properties

`SupportedFeatures`

ManagementServerCapabilitiesSupportedFeaturesObject

 (Required) 

A dictionary that contains the server’s optional protocol features.

Each dictionary item uses the key name to represent a feature, and the value to hold the feature’s associated parameters. This protocol reserves keys with a prefix of “`com.apple.`”, which appear as subkeys in this dictionary.

`Version`

`string`

 (Required) 

The server’s protocol version.

## Mentioned in 

Leveraging the declarative management data model to scale devices

## Discussion

Specify `com.apple.management.server-capabilities` as the declaration type.

## Topics

### Supporting Objects

object ManagementServerCapabilitiesSupportedFeaturesObject

A dictionary that contains the server’s optional protocol features.

## See Also

### Management

object ManagementOrganizationInformation

The declaration to configure the managing organization’s contact information.

object ManagementProperties

The declaration to configure the properties on the device.

