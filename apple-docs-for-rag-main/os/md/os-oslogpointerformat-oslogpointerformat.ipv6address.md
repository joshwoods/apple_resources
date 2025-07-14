

- os
- OSLogPointerFormat
-  OSLogPointerFormat.ipv6Address 

Case

# OSLogPointerFormat.ipv6Address

An option to display the pointer bytes as an IPv6 network address.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
case ipv6Address
```

## Discussion

This option formats an `in6_addr` structure as an easily readable string.

## See Also

### Getting the Format Options

case none

An option to treat the pointer as raw bytes, and not format it.

case sockaddr

An option to display the pointer bytes as a socket address.

case timespec

An option to display the pointer bytes as a time specification.

case timeval

An option to display the pointer bytes as a time value.

case uuid

An option to display the pointer bytes as a formatted UUID.

