

- Foundation
- PredicateExpressions
-  PredicateExpressions.Range 

Structure

# PredicateExpressions.Range

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct Range where LHS : PredicateExpression, RHS : PredicateExpression, LHS.Output : Comparable, LHS.Output == RHS.Output
```

## Topics

### Initializers

init(lower: LHS, upper: RHS)

### Instance Properties

let lower: LHS

let upper: RHS

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- PredicateExpression
- Sendable
- StandardPredicateExpression

  Conforms when `LHS` conforms to `StandardPredicateExpression`, `RHS` conforms to `StandardPredicateExpression`, `LHS.Output` conforms to `Comparable`, and `LHS.Output` is `RHS.Output`.

