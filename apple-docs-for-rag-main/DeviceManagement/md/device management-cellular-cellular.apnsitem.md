

- Device Management
- Cellular
-  Cellular.APNsItem 

Device Management Profile

# Cellular.APNsItem

A dictionary that contains details about an access point name (APN) configuration.

iOS 7.0+iPadOS 7.0+watchOS 3.2+Device Assignment ServicesVPP License Management

``` source
object Cellular.APNsItem
```

## Properties

`AllowedProtocolMask`

`integer`

The Internet Protocol versions that the system supports. Available in iOS 10.3 and later. Allowed values:

- `1`: IPv4

- `2`: IPv6

- `3`: Both

Possible Values: `1, 2, 3`

`AllowedProtocolMaskInDomesticRoaming`

`integer`

The Internet Protocol versions that the system supports while roaming. Available in iOS 10.3 and later. Allowed values:

- `1`: IPv4

- `2`: IPv6

- `3`: Both

Possible Values: `1, 2, 3`

`AllowedProtocolMaskInRoaming`

`integer`

The Internet Protocol versions that the system supports while roaming. Available in iOS 10.3 and later. Allowed values:

- `1`: IPv4

- `2`: IPv6

- `3`: Both

Possible Values: `1, 2, 3`

`AuthenticationType`

`string`

The authentication type for logging in.

Default: `PAP`

Possible Values: `CHAP, PAP`

`EnableXLAT464`

`boolean`

If `true`, the system enables XLAT464. Available in iOS 16 and later and watchOS 9 and later.

Default: `false`

`Name`

`string`

 (Required) 

The name for this configuration.

`Password`

`string`

The user’s password for the APN.

`ProxyPort`

`integer`

The proxy server’s port number.

`ProxyServer`

`string`

The proxy server’s address.

`Username`

`string`

The user name for the APN.

`DefaultProtocolMask`

`integer`

Deprecated 

The default Internet Protocol versions. Available in iOS 10.3 but no longer used in iOS 11 and later. Allowed values:

- `1`: IPv4

- `2`: IPv6

- `3`: Both

Possible Values: `1, 2, 3`

## See Also

### Objects

object Cellular.AttachAPN

A dictionary that contains details about an attach access point name (APN) configuration.

