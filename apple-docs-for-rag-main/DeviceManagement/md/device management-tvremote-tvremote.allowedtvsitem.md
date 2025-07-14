

- Device Management
- TVRemote
-  TVRemote.AllowedTVsItem 

Device Management Profile

# TVRemote.AllowedTVsItem

The array of valid Apple TV identifiers that the remote can connect to.

iOS 11.3+iPadOS 11.3+tvOS 11.3+Device Assignment ServicesVPP License Management

``` source
object TVRemote.AllowedTVsItem
```

## Properties

`TVDeviceID`

`string`

 (Required) 

The MAC address of an Apple TV device that the system permits this iOS device to control. Use the format `xx:xx:xx:xx:xx:xx`, which isn’t case-sensitive.

`TVDeviceName`

`string`

The name of an Apple TV device that the system permits this iOS device to control.

## See Also

### Objects

object TVRemote.AllowedRemotesItem

The array of valid devices that Apple TV can connect to.

