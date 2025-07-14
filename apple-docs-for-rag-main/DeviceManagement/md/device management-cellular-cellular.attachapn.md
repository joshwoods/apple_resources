

- Device Management
- Cellular
-  Cellular.AttachAPN 

Device Management Profile

# Cellular.AttachAPN

A dictionary that contains details about an attach access point name (APN) configuration.

iOS 7.0+iPadOS 7.0+watchOS 3.2+Device Assignment ServicesVPP License Management

``` source
object Cellular.AttachAPN
```

## Properties

`AllowedProtocolMask`

`integer`

The Internet Protocol versions that the system supports. Allowed values:

- `1`: IPv4

- `2`: IPv6

- `3`: Both

Possible Values: `1, 2, 3`

`AuthenticationType`

`string`

The authentication type.

Default: `PAP`

Possible Values: `CHAP, PAP`

`Name`

`string`

 (Required) 

The name for this configuration.

`Password`

`string`

The password for the user.

`Username`

`string`

The user name.

## See Also

### Objects

object Cellular.APNsItem

A dictionary that contains details about an access point name (APN) configuration.

