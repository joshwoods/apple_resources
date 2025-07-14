

- Device Management
- AirPlay
-  AirPlay.PasswordsItem 

Device Management Profile

# AirPlay.PasswordsItem

The dictionary that defines passwords for AirPlay destinations.

iOS 7.0+iPadOS 7.0+macOS 10.10+Device Assignment ServicesVPP License Management

``` source
object AirPlay.PasswordsItem
```

## Properties

`DeviceID`

`string`

Deprecated 

The device ID of the AirPlay destination; used in macOS.

In tvOS 18 and later, `DeviceID` is deprecated; use `DeviceName` instead.

`DeviceName`

`string`

 (Required) 

The name of the AirPlay destination; used in iOS, and available in macOS 15 and later.

`Password`

`string`

 (Required) 

The password for the AirPlay destination.

## See Also

### Supporting Objects

object AirPlay.AllowListItem

The dictionary that defines allowed destinations.

