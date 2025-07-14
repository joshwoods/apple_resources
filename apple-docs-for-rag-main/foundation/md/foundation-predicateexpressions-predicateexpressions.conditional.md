

- Foundation
- PredicateExpressions
-  PredicateExpressions.Conditional 

Structure

# PredicateExpressions.Conditional

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct Conditional where Test : PredicateExpression, If : PredicateExpression, Else : PredicateExpression, Test.Output == Bool, If.Output == Else.Output
```

## Topics

### Initializers

init(test: Test, trueBranch: If, falseBranch: Else)

### Instance Properties

let falseBranch: Else

let test: Test

let trueBranch: If

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- PredicateExpression
- Sendable
- StandardPredicateExpression

  Conforms when `Test` conforms to `StandardPredicateExpression`, `If` conforms to `StandardPredicateExpression`, `Else` conforms to `StandardPredicateExpression`, `Test.Output` is `Bool`, and `If.Output` is `Else.Output`.

