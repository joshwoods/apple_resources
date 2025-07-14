

- Foundation
- PredicateExpressions
-  PredicateExpressions.CollectionRangeSubscript 

Structure

# PredicateExpressions.CollectionRangeSubscript

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct CollectionRangeSubscript where Wrapped : PredicateExpression, Range : PredicateExpression, Wrapped.Output : Collection, Range.Output == Range
```

## Topics

### Initializers

init(wrapped: Wrapped, range: Range)

### Instance Properties

let range: Range

let wrapped: Wrapped

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- PredicateExpression
- Sendable
- StandardPredicateExpression

  Conforms when `Wrapped` conforms to `StandardPredicateExpression`, `Range` conforms to `StandardPredicateExpression`, `Wrapped.Output` conforms to `Collection`, and `Range.Output` is `Range`.

