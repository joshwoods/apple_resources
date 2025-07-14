

- Swift
- Unicode
- Unicode.UTF32
-  Unicode.UTF32.Parser 

Structure

# Unicode.UTF32.Parser

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct Parser
```

## Topics

### Initializers

init()

Constructs an instance that can be used to begin parsing `CodeUnit`s at any Unicode scalar boundary.

### Instance Methods

func parseScalar&lt;I>(from: inout I) -> Unicode.ParseResult&lt;Unicode.UTF32.Parser.Encoding.EncodedScalar>

Parses a single Unicode scalar value from `input`.

### Type Aliases

typealias Encoding

The encoding with which this parser is associated

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Sendable

