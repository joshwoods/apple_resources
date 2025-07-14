

- os
-  OSLogPointerFormat 

Enumeration

# OSLogPointerFormat

The formatting options for pointer data.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
enum OSLogPointerFormat
```

## Mentioned in 

Generating Log Messages from Your Code

## Topics

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

case uuid

An option to display the pointer bytes as a formatted UUID.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Value Formatters

enum OSLogBoolFormat

The formatting options for Boolean values.

struct OSLogIntegerFormatting

The formatting options for integer values.

enum OSLogInt32ExtendedFormat

The formatting options for 32-bit integer values.

struct OSLogFloatFormatting

The formatting options for double and floating-point numbers.

