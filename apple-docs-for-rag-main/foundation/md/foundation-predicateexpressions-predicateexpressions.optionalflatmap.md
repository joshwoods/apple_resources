

- Foundation
- PredicateExpressions
-  PredicateExpressions.OptionalFlatMap 

Structure

# PredicateExpressions.OptionalFlatMap

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct OptionalFlatMap where LHS : PredicateExpression, RHS : PredicateExpression, LHS.Output == Wrapped?
```

## Topics

### Initializers

init(LHS, (PredicateExpressions.Variable&lt;Wrapped>) -> RHS)

init(LHS, (PredicateExpressions.Variable&lt;Wrapped>) -> RHS)

### Instance Properties

let transform: RHS

let variable: PredicateExpressions.Variable&lt;Wrapped>

let wrapped: LHS

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- PredicateExpression
- Sendable
- StandardPredicateExpression

  Conforms when `LHS` conforms to `StandardPredicateExpression`, `Wrapped` conforms to `Copyable`, `Wrapped` conforms to `Escapable`, `RHS` conforms to `StandardPredicateExpression`, `Result` conforms to `Copyable`, `Result` conforms to `Escapable`, and `LHS.Output` is `Wrapped?`.

