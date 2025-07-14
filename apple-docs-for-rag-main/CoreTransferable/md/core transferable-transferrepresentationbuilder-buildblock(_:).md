

- Core Transferable
- TransferRepresentationBuilder
-  buildBlock(\_:) 

Type Method

# buildBlock(\_:)

Passes a single transfer representation to the builder unmodified.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func buildBlock(_ content: Content) -> Content where Item == Content.Item, Content : TransferRepresentation
```

## See Also

### Building a transfer representation

static func buildExpression&lt;R>(R) -> R

Builds a transfer representation from an expression.

static func buildExpression&lt;Encoder, Decoder>(CodableRepresentation&lt;Item, Encoder, Decoder>) -> CodableRepresentation&lt;Item, Encoder, Decoder>

Builds an encodable and decodable transfer representation from an expression.

