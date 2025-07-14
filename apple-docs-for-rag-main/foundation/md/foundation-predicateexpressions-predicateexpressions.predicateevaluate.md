

- Foundation
- PredicateExpressions
-  PredicateExpressions.PredicateEvaluate 

Structure

# PredicateExpressions.PredicateEvaluate

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.0+watchOS 10.4+

``` source
struct PredicateEvaluate where Condition : PredicateExpression, repeat each Input : PredicateExpression, Condition.Output == Predicate
```

## Topics

### Initializers

init(predicate: Condition, input: repeat each Input)

### Instance Properties

let input: (repeat each Input)

let predicate: Condition

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- PredicateExpression
- Sendable
- StandardPredicateExpression

  Conforms when `Condition` conforms to `StandardPredicateExpression`, `each Input` conforms to `StandardPredicateExpression`, and `Condition.Output` is `Predicate`.

