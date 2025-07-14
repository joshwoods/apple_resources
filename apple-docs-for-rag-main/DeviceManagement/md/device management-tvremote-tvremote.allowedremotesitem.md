

- Device Management
- TVRemote
-  TVRemote.AllowedRemotesItem 

Device Management Profile

# TVRemote.AllowedRemotesItem

The array of valid devices that Apple TV can connect to.

iOS 11.3+iPadOS 11.3+tvOS 11.3+Device Assignment ServicesVPP License Management

``` source
object TVRemote.AllowedRemotesItem
```

## Properties

`RemoteDeviceID`

`string`

 (Required) 

The MAC address of a permitted iOS device that can control this Apple TV. Use the format `xx:xx:xx:xx:xx:xx`, which isn’t case-sensitive.

## See Also

### Objects

object TVRemote.AllowedTVsItem

The array of valid Apple TV identifiers that the remote can connect to.

