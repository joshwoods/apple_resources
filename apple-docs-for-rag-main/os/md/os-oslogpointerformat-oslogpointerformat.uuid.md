

- os
- OSLogPointerFormat
-  OSLogPointerFormat.uuid 

Case

# OSLogPointerFormat.uuid

An option to display the pointer bytes as a formatted UUID.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
case uuid
```

## Discussion

This option prints an easily readable uuid_t type.

## See Also

### Getting the Format Options

case none

An option to treat the pointer as raw bytes, and not format it.

case ipv6Address

An option to display the pointer bytes as an IPv6 network address.

case sockaddr

An option to display the pointer bytes as a socket address.

case timespec

An option to display the pointer bytes as a time specification.

case timeval

An option to display the pointer bytes as a time value.

