

- Device Management
- ContentCaching
-  ContentCaching.Ranges 

Device Management Profile

# ContentCaching.Ranges

A range of IP addresses to cache.

macOS 10.13.4+Device Assignment ServicesVPP License Management

``` source
object ContentCaching.Ranges
```

## Properties

`first`

`string`

 (Required) 

The first IP address in the range.

`last`

`string`

 (Required) 

The last IP address in the range.

`type`

`string`

The IP address type.

Default: `IPv4`

Possible Values: `IPv4, IPv6`

