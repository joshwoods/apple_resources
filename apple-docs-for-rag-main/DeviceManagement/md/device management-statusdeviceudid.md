

- Device Management
-  StatusDeviceUDID 

Object

# StatusDeviceUDID

A status report of the device’s UDID.

iOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object StatusDeviceUDID
```

## Properties

`device.identifier.udid`

`string`

 (Required) 

The device’s UDID. This value is always available on the device channel. This value is only available on user channels whose organization matches that of the device channel.

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

object StatusDiskManagementFileVaultEnabled

The enabled status of the File Vault.

object StatusManagementClientCapabilities

A status report of the client’s protocol capabilities.

