

- Core Transferable
- TransferRepresentationBuilder
-  buildExpression(\_:) 

Type Method

# buildExpression(\_:)

Builds an encodable and decodable transfer representation from an expression.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func buildExpression(_ content: CodableRepresentation) -> CodableRepresentation where Item : Decodable, Item : Encodable, Encoder : TopLevelEncoder, Decoder : TopLevelDecoder, Encoder.Output == Data, Decoder.Input == Data
```

## See Also

### Building a transfer representation

static func buildBlock&lt;Content>(Content) -> Content

Passes a single transfer representation to the builder unmodified.

static func buildExpression&lt;R>(R) -> R

Builds a transfer representation from an expression.

