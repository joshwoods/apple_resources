

- Foundation
- PredicateExpressions
-  PredicateExpressions.CollectionIndexSubscript 

Structure

# PredicateExpressions.CollectionIndexSubscript

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct CollectionIndexSubscript where Wrapped : PredicateExpression, Index : PredicateExpression, Wrapped.Output : Collection, Index.Output == Wrapped.Output.Index
```

## Topics

### Initializers

init(wrapped: Wrapped, index: Index)

### Instance Properties

let index: Index

let wrapped: Wrapped

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- PredicateExpression

  Conforms when `Wrapped` conforms to `StandardPredicateExpression`, `Index` conforms to `StandardPredicateExpression`, `Wrapped.Output` conforms to `Collection`, and `Index.Output` is `Wrapped.Output.Index`.

- Sendable
- StandardPredicateExpression

  Conforms when `Wrapped` conforms to `StandardPredicateExpression`, `Index` conforms to `StandardPredicateExpression`, `Wrapped.Output` conforms to `Collection`, and `Index.Output` is `Wrapped.Output.Index`.

