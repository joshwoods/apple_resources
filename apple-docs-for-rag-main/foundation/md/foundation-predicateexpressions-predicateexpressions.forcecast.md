

- Foundation
- PredicateExpressions
-  PredicateExpressions.ForceCast 

Structure

# PredicateExpressions.ForceCast

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct ForceCast where Input : PredicateExpression
```

## Topics

### Initializers

init(Input)

### Instance Properties

let input: Input

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- PredicateExpression
- Sendable
- StandardPredicateExpression

  Conforms when `Input` conforms to `StandardPredicateExpression`, `Desired` conforms to `Copyable`, and `Desired` conforms to `Escapable`.

