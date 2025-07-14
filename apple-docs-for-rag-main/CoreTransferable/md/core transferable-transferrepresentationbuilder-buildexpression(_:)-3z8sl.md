

- Core Transferable
- TransferRepresentationBuilder
-  buildExpression(\_:) 

Type Method

# buildExpression(\_:)

Builds a transfer representation from an expression.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func buildExpression(_ content: R) -> R where Item == R.Item, R : TransferRepresentation
```

## See Also

### Building a transfer representation

static func buildBlock&lt;Content>(Content) -> Content

Passes a single transfer representation to the builder unmodified.

static func buildExpression&lt;Encoder, Decoder>(CodableRepresentation&lt;Item, Encoder, Decoder>) -> CodableRepresentation&lt;Item, Encoder, Decoder>

Builds an encodable and decodable transfer representation from an expression.

