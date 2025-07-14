

- Foundation
- PredicateExpressions
-  PredicateExpressions.ExpressionEvaluate 

Structure

# PredicateExpressions.ExpressionEvaluate

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 1.0+watchOS 11.0+

``` source
struct ExpressionEvaluate where Transformation : PredicateExpression, repeat each Input : PredicateExpression, Transformation.Output == Expression
```

## Topics

### Initializers

init(expression: Transformation, input: repeat each Input)

### Instance Properties

let expression: Transformation

let input: (repeat each Input)

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- PredicateExpression
- Sendable
- StandardPredicateExpression

  Conforms when `Transformation` conforms to `StandardPredicateExpression`, `each Input` conforms to `StandardPredicateExpression`, `Output` conforms to `Copyable`, `Output` conforms to `Escapable`, and `Transformation.Output` is `Expression`.

