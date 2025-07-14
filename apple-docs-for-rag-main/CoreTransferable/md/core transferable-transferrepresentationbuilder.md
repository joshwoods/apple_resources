

- Core Transferable
-  TransferRepresentationBuilder 

Structure

# TransferRepresentationBuilder

Creates a transfer representation by composing existing transfer representations.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@resultBuilder
struct TransferRepresentationBuilder where Item : Transferable
```

## Topics

### Building a transfer representation

static func buildBlock&lt;Content>(Content) -> Content

Passes a single transfer representation to the builder unmodified.

static func buildExpression&lt;R>(R) -> R

Builds a transfer representation from an expression.

static func buildExpression&lt;Encoder, Decoder>(CodableRepresentation&lt;Item, Encoder, Decoder>) -> CodableRepresentation&lt;Item, Encoder, Decoder>

Builds an encodable and decodable transfer representation from an expression.

### Combining transfer representations

static func buildBlock&lt;C1, C2>(C1, C2) -> TupleTransferRepresentation&lt;Item, (C1, C2)>

Combines multiple transfer representations into a single transfer representation.

static func buildBlock&lt;C1, C2, C3>(C1, C2, C3) -> TupleTransferRepresentation&lt;Item, (C1, C2, C3)>

Combines multiple transfer representations into a single transfer representation.

static func buildBlock&lt;C1, C2, C3, C4>(C1, C2, C3, C4) -> TupleTransferRepresentation&lt;Item, (C1, C2, C3, C4)>

Combines multiple transfer representations into a single transfer representation.

static func buildBlock&lt;C1, C2, C3, C4, C5>(C1, C2, C3, C4, C5) -> TupleTransferRepresentation&lt;Item, (C1, C2, C3, C4, C5)>

Combines multiple transfer representations into a single transfer representation.

static func buildBlock&lt;C1, C2, C3, C4, C5, C6>(C1, C2, C3, C4, C5, C6) -> TupleTransferRepresentation&lt;Item, (C1, C2, C3, C4, C5, C6)>

Combines multiple transfer representations into a single transfer representation.

static func buildBlock&lt;C1, C2, C3, C4, C5, C6, C7>(C1, C2, C3, C4, C5, C6, C7) -> TupleTransferRepresentation&lt;Item, (C1, C2, C3, C4, C5, C6, C7)>

Combines multiple transfer representations into a single transfer representation.

static func buildBlock&lt;C1, C2, C3, C4, C5, C6, C7, C8>(C1, C2, C3, C4, C5, C6, C7, C8) -> TupleTransferRepresentation&lt;Item, (C1, C2, C3, C4, C5, C6, C7, C8)>

Combines multiple transfer representations into a single transfer representation.

static func buildBlock&lt;C1, C2, C3, C4, C5, C6, C7, C8, C9>(C1, C2, C3, C4, C5, C6, C7, C8, C9) -> TupleTransferRepresentation&lt;Item, (C1, C2, C3, C4, C5, C6, C7, C8, C9)>

Combines multiple transfer representations into a single transfer representation.

static func buildBlock&lt;C1, C2, C3, C4, C5, C6, C7, C8, C9, C10>(C1, C2, C3, C4, C5, C6, C7, C8, C9, C10) -> TupleTransferRepresentation&lt;Item, (C1, C2, C3, C4, C5, C6, C7, C8, C9, C10)>

Combines multiple transfer representations into a single transfer representation.

## See Also

### Supporting types

struct TupleTransferRepresentation

A wrapper type for tuples that contain transfer representations.

