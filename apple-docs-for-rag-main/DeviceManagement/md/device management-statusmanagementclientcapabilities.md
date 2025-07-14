

- Device Management
-  StatusManagementClientCapabilities 

Object

# StatusManagementClientCapabilities

A status report of the client’s protocol capabilities.

iOS 15.0+iPadOS 15.0+macOS 13.0+tvOS 16.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object StatusManagementClientCapabilities
```

## Properties

`management.client-capabilities`

StatusManagementClientCapabilitiesCapabilitiesObject

 (Required) 

An object that contains the client’s protocol capabilities. These typically only change when the device upgrades its software. An implicit status subscription for this status item is always present, so the client always reports changes to the server.

## Mentioned in 

Leveraging the declarative management data model to scale devices

## Topics

### Supporting Objects

object StatusManagementClientCapabilitiesCapabilitiesObject

A collection of the device’s supported features, payloads, and versions.

object StatusManagementClientCapabilitiesCapabilities_SupportedFeaturesObject

A set of optional protocol features that the client supports.

object StatusManagementClientCapabilitiesCapabilities_SupportedPayloadsObject

The set of declaration and status items that the client supports.

object StatusManagementClientCapabilitiesCapabilities_SupportedPayloads_DeclarationsObject

A declaration that the client supports.

## See Also

### Status Reports and Elements

object StatusReport

A status report of the device’s current state.

object StatusAppManagedList

The device’s declarative managed apps.

object StatusDeviceBatteryHealth

The device’s battery health.

object StatusDeviceModelFamily

A status report of the device’s hardware family.

object StatusDeviceModelIdentifier

A status report of the device’s hardware identifier.

object StatusDeviceModelMarketingName

A status report of the device’s marketing name.

object StatusDeviceModelNumber

A status report of the device’s hardware number.

object StatusDeviceOperatingSystemBuildVersion

A status report of the device’s software build identifier.

object StatusDeviceOperatingSystemFamily

A status report of the device’s operating system family.

object StatusDeviceOperatingSystemSupplementalBuildVersion

A status report of the device’s operating system supplemental build identifier.

object StatusDeviceOperatingSystemSupplementalExtraVersion

A status report of the device’s operating system’s rapid security response identifier.

object StatusDeviceOperatingSystemVersion

A status report of the device’s operating system version.

object StatusDeviceSerialNumber

A status report of the device’s serial number.

object StatusDeviceUDID

A status report of the device’s UDID.

object StatusDiskManagementFileVaultEnabled

The enabled status of the File Vault.

