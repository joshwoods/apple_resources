

- Device Management
-  StatusAppManagedList 

Object

# StatusAppManagedList

The device’s declarative managed apps.

iOS 17.2+iPadOS 17.2+visionOS 2.4+Device Assignment ServicesVPP License Management

``` source
object StatusAppManagedList
```

## Properties

`app.managed.list`

`[`StatusAppManagedListAppObject`]`

 (Required) 

An array of dictionaries that describe the device’s declarative managed apps.

## Discussion

Note

This documentation contains preliminary information about an API or technology in development. This information is subject to change. Learn more about using Apple’s beta software.

## Topics

### Objects

object StatusAppManagedListAppObject

A dictionary that describes a declarative managed app.

## See Also

### Status Reports and Elements

object StatusReport

A status report of the device’s current state.

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

object StatusManagementClientCapabilities

A status report of the client’s protocol capabilities.

