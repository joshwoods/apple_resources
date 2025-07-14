

- Device Management
-  StatusManagementDeclarations 

Object

# StatusManagementDeclarations

A status report of the client’s processed declarations.

iOS 15.0+iPadOS 15.0+macOS 13.0+tvOS 16.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object StatusManagementDeclarations
```

## Properties

`management.declarations`

StatusManagementDeclarationsDeclarationsObject

 (Required) 

A collection of the client’s processed declarations.

## Discussion

The name of the declaration status item is `management.declarations`.

## Topics

### Supporting Objects

object StatusManagementDeclarationsDeclarationsObject

A collection of the client’s processed declarations.

object StatusManagementDeclarationsDeclarationObject

A processed declaration for the client.

object StatusManagementDeclarationsStatusReasonObject

The details of an error in a status report.

object StatusManagementDeclarationsStatusReason_DetailsObject

A dictionary that contains further details about an error.

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

