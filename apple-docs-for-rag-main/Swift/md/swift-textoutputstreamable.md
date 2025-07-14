

- Swift
-  TextOutputStreamable 

Protocol

# TextOutputStreamable

A source of text-streaming operations.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol TextOutputStreamable
```

## Overview

Instances of types that conform to the `TextOutputStreamable` protocol can write their value to instances of any type that conforms to the `TextOutputStream` protocol. The Swift standard library’s text-related types, `String`, `Character`, and `Unicode.Scalar`, all conform to `TextOutputStreamable`.

# Conforming to the TextOutputStreamable Protocol

To add `TextOutputStreamable` conformance to a custom type, implement the required `write(to:)` method. Call the given output stream’s `write(_:)` method in your implementation.

## Topics

### Instance Methods

func write&lt;Target>(to: inout Target)

Writes a textual representation of this instance into the given output stream.

**Required**

## Relationships

### Inherited By

- StringProtocol

### Conforming Types

- Character
- Double
- Float
- Float16
- Float80
- String
- Substring
- Unicode.Scalar

## See Also

### Streams

protocol TextOutputStream

A type that can be the target of text-streaming operations.

