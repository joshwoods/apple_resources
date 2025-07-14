

- Swift
- Unicode
- Unicode.ASCII
-  Unicode.ASCII.Parser 

Structure

# Unicode.ASCII.Parser

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

func parseScalar&lt;I>(from: inout I) -> Unicode.ParseResult&lt;Unicode.ASCII.Parser.Encoding.EncodedScalar>

Parses a single Unicode scalar value from `input`.

### Type Aliases

typealias Encoding

The encoding with which this parser is associated

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Sendable

