

- Metal
-  MTLCompareFunction 

Enumeration

# MTLCompareFunction

Options used to specify how a sample compare operation should be performed on a depth texture.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
enum MTLCompareFunction
```

## Overview

Whenever the comparison test passes, the incoming fragment is compared to the stored data at the specified location.

## Topics

### Compare function options

case never

A new value never passes the comparison test.

case less

A new value passes the comparison test if it is less than the existing value.

case equal

A new value passes the comparison test if it is equal to the existing value.

case lessEqual

A new value passes the comparison test if it is less than or equal to the existing value.

case greater

A new value passes the comparison test if it is greater than the existing value.

case notEqual

A new value passes the comparison test if it is not equal to the existing value.

case greaterEqual

A new value passes the comparison test if it is greater than or equal to the existing value.

case always

A new value always passes the comparison test.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Declaring the Depth Comparison Mode

var compareFunction: MTLCompareFunction

The sampler comparison function used when performing a sample compare operation on a depth texture.

