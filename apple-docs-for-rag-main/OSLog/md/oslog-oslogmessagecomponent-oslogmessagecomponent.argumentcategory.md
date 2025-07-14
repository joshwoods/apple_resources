

- OSLog
- OSLogMessageComponent
-  OSLogMessageComponent.ArgumentCategory 

Enumeration

# OSLogMessageComponent.ArgumentCategory

The data type corresponding to the argument provided in a message payload.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum ArgumentCategory
```

## Overview

For example, `OSLogMessageComponent` can represent the number associated with a `%d` placeholder. This value can be undefined if the argument data cann’t be decoded, for example if it were redacted.

## Topics

### Constants

case data

The argument is an NSData object.

case double

The argument is a double.

case int64

The argument is a 64-bit signed integer.

case string

The argument is a string.

case uInt64

The argument is a 64-bit unsigned integer.

case undefined

The argument’s type is not defined.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Reading the Argument

var argument: OSLogMessageComponent.Argument

The argument passed into the message component.

enum Argument

An object representing data that corresponds to an argument in a message payload.

var argumentCategory: OSLogMessageComponent.ArgumentCategory

The type of argument that corresponds to the placeholder.

