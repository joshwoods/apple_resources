

- Foundation
- PredicateExpressions
-  PredicateExpressions.Comparison 

Structure

# PredicateExpressions.Comparison

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct Comparison where LHS : PredicateExpression, RHS : PredicateExpression, LHS.Output : Comparable, LHS.Output == RHS.Output
```

## Topics

### Initializers

init(lhs: LHS, rhs: RHS, op: PredicateExpressions.ComparisonOperator)

### Instance Properties

let lhs: LHS

let op: PredicateExpressions.ComparisonOperator

let rhs: RHS

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

