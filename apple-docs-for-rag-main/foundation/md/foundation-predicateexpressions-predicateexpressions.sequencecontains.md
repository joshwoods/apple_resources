

- Foundation
- PredicateExpressions
-  PredicateExpressions.SequenceContains 

Structure

# PredicateExpressions.SequenceContains

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct SequenceContains where LHS : PredicateExpression, RHS : PredicateExpression, LHS.Output : Sequence, RHS.Output : Equatable, RHS.Output == LHS.Output.Element
```

## Topics

### Initializers

init(sequence: LHS, element: RHS)

### Instance Properties

let element: RHS

let sequence: LHS

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- PredicateExpression
- Sendable
- StandardPredicateExpression

  Conforms when `LHS` conforms to `StandardPredicateExpression`, `RHS` conforms to `StandardPredicateExpression`, `LHS.Output` conforms to `Sequence`, `RHS.Output` conforms to `Equatable`, and `RHS.Output` is `LHS.Output.Element`.

