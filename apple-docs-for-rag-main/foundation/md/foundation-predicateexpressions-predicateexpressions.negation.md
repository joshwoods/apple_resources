

- Foundation
- PredicateExpressions
-  PredicateExpressions.Negation 

Structure

# PredicateExpressions.Negation

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct Negation where Wrapped : PredicateExpression, Wrapped.Output == Bool
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

  Conforms when `Wrapped` conforms to `StandardPredicateExpression` and `Wrapped.Output` is `Bool`.

