

- Swift
- Unicode
- Unicode.UTF8
-  Unicode.UTF8.ReverseParser 

Structure

# Unicode.UTF8.ReverseParser

A type that can be used to parse a reversed sequence of `CodeUnits` into `EncodedScalar`s.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct ReverseParser
```

## Topics

### Initializers

init()

Constructs an instance that can be used to begin parsing `CodeUnit`s at any Unicode scalar boundary.

### Type Aliases

typealias Encoding

The encoding with which this parser is associated

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Sendable

