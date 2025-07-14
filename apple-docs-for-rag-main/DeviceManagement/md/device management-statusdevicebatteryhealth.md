

- Device Management
-  StatusDeviceBatteryHealth 

Object

# StatusDeviceBatteryHealth

The device’s battery health.

iOS 17.0+iPadOS 17.0+macOS 14.4+Device Assignment ServicesVPP License Management

``` source
object StatusDeviceBatteryHealth
```

## Properties

`device.power.battery-health`

`string`

 (Required) 

The battery health status, which has the following values:

`non-genuine`  
The battery isn’t a genuine Apple battery.

Possible Values: `non-genuine, normal, service-recommended, unknown, unsupported`

## Overview

`normal`  
The battery is operating normally.

`service-recommended`  
The system recommends battery service.

`unknown`  
The system couldn’t determine battery health information.

`unsupported`  
The device doesn’t support battery health reporting.

Available in iOS 17 and later on iPhone only (iPad returns `unsupported`), and macOS 14.4 and later on Apple silicon Mac computers.

## See Also

### Status Reports and Elements

object StatusReport

A status report of the device’s current state.

object StatusAppManagedList

The device’s declarative managed apps.

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

