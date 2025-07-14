

- Device Management
-  StatusDeviceModelIdentifier 

Object

# StatusDeviceModelIdentifier

A status report of the device’s hardware identifier.

iOS 15.0+iPadOS 15.0+macOS 13.0+tvOS 16.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object StatusDeviceModelIdentifier
```

## Properties

`device.model.identifier`

`string`

 (Required) 

A two-part string that specifies the device’s model. The first part specifies device’s model family, and the second part specifies the model’s version. The model’s version is a comma-separated number where the first part of the number is the version, and the second part is a variant, such as `MacBookPro15,1` or `iPhone13,2`.

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

object StatusManagementClientCapabilities

A status report of the client’s protocol capabilities.

