

- Foundation
- PredicateExpressions
-  PredicateExpressions.Filter 

Structure

# PredicateExpressions.Filter

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct Filter where LHS : PredicateExpression, RHS : PredicateExpression, LHS.Output : Sequence, RHS.Output == Bool
```

## Topics

### Initializers

init(LHS, (PredicateExpressions.Variable&lt;PredicateExpressions.Filter&lt;LHS, RHS>.Element>) -> RHS)

### Instance Properties

let filter: RHS

let sequence: LHS

let variable: PredicateExpressions.Variable&lt;PredicateExpressions.Filter&lt;LHS, RHS>.Element>

### Type Aliases

typealias Element

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- PredicateExpression
- Sendable
- StandardPredicateExpression

  Conforms when `LHS` conforms to `StandardPredicateExpression`, `RHS` conforms to `StandardPredicateExpression`, `LHS.Output` conforms to `Sequence`, and `RHS.Output` is `Bool`.

