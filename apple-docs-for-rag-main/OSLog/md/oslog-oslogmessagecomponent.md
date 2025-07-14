

- OSLog
-  OSLogMessageComponent 

Class

# OSLogMessageComponent

The message arguments for a particular entry.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class OSLogMessageComponent
```

## Overview

There is one component for each placeholder in the formatString plus one component for any text after the last placeholder.

## Topics

### Reading the Argument

var argument: OSLogMessageComponent.Argument

The argument passed into the message component.

enum Argument

An object representing data that corresponds to an argument in a message payload.

var argumentCategory: OSLogMessageComponent.ArgumentCategory

The type of argument that corresponds to the placeholder.

enum ArgumentCategory

The data type corresponding to the argument provided in a message payload.

### Reading the Message Component

var formatSubstring: String

The text immediately preceding a placeholder.

var placeholder: String

The placeholder text for the message component.

### Accessing the Argument

var argumentDataValue: Data?

The argument formatted as a sequence of bytes.

var argumentDoubleValue: Double

The argument formatted as a double.

var argumentInt64Value: Int64

The argument formatted as a signed 64-bit integer.

var argumentNumberValue: NSNumber?

The argument formatted as a number.

var argumentStringValue: String?

The argument formatted as a string.

var argumentUInt64Value: UInt64

The argument formatted as an unsigned 64-bit integer.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Entry Data

class OSLogPosition

A representation of a point in a sequence of entries in the unified logging system.

