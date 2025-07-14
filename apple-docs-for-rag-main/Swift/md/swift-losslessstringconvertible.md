

- Swift
-  LosslessStringConvertible 

Protocol

# LosslessStringConvertible

A type that can be represented as a string in a lossless, unambiguous way.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol LosslessStringConvertible : CustomStringConvertible
```

## Overview

For example, the integer value 1050 can be represented in its entirety as the string “1050”.

The description property of a conforming type must be a value-preserving representation of the original value. As such, it should be possible to re-create an instance from its string representation.

## Topics

### Initializers

init?(String)

Instantiates an instance of the conforming type from a string representation.

**Required** Default implementations provided.

## Relationships

### Inherits From

- CustomStringConvertible

### Inherited By

- FixedWidthInteger
- StringProtocol

### Conforming Types

- Bool
- Character
- Double
- Float
- Float16
- Float80
- Int
- Int128
- Int16
- Int32
- Int64
- Int8
- String
- Substring
- UInt
- UInt128
- UInt16
- UInt32
- UInt64
- UInt8
- Unicode.Scalar

## See Also

### String Representation

protocol CustomStringConvertible

A type with a customized textual representation.

protocol CustomDebugStringConvertible

A type with a customized textual representation suitable for debugging purposes.

