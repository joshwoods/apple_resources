

- Device Management
- AirPlay
-  AirPlay.AllowListItem 

Device Management Profile

# AirPlay.AllowListItem

The dictionary that defines allowed destinations.

iOS 7.0+iPadOS 7.0+macOS 10.10+Device Assignment ServicesVPP License Management

``` source
object AirPlay.AllowListItem
```

## Properties

`DeviceID`

`string`

Deprecated 

The device ID of the AirPlay destination in the format `xx:xx:xx:xx:xx:xx`. This field isn’t case-sensitive.

The system limits the list of visible AirPlay destinations to devices that are present in the `AllowList` field of all installed AirPlay payloads.

Specifying the same MACAddress more than once, whether in the same payload across different payloads, results in undefined behavior.

As of tvOS 18, `DeviceID` isn’t supported.

`DeviceName`

`string`

The name of the AirPlay device.

The system limits the list of visible AirPlay destinations to devices that are present in the `AllowList` field of all installed AirPlay payloads.

## See Also

### Supporting Objects

object AirPlay.PasswordsItem

The dictionary that defines passwords for AirPlay destinations.

