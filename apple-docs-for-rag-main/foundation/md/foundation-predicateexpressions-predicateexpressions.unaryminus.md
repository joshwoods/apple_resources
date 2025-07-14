

- Foundation
- PredicateExpressions
-  PredicateExpressions.UnaryMinus 

Structure

# PredicateExpressions.UnaryMinus

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct UnaryMinus where Wrapped : PredicateExpression, Wrapped.Output : SignedNumeric
```

## Topics

### Initializers

init(Wrapped)

### Instance Properties

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

  Conforms when `Wrapped` conforms to `StandardPredicateExpression` and `Wrapped.Output` conforms to `SignedNumeric`.

