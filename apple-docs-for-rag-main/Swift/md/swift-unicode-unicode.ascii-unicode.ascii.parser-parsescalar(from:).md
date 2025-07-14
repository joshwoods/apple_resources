

- Swift
- Unicode
- Unicode.ASCII
- Unicode.ASCII.Parser
-  parseScalar(from:) 

Instance Method

# parseScalar(from:)

Parses a single Unicode scalar value from `input`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func parseScalar(from input: inout I) -> Unicode.ParseResult where I : IteratorProtocol, I.Element == UInt8
```

