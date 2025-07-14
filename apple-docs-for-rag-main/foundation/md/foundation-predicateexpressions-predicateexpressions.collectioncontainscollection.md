

- Foundation
- PredicateExpressions
-  PredicateExpressions.CollectionContainsCollection 

Structure

# PredicateExpressions.CollectionContainsCollection

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct CollectionContainsCollection where Base : PredicateExpression, Other : PredicateExpression, Base.Output : Collection, Other.Output : Collection, Base.Output.Element : Equatable, Base.Output.Element == Other.Output.Element
```

## Topics

### Initializers

init(base: Base, other: Other)

### Instance Properties

let base: Base

let other: Other

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- PredicateExpression
- Sendable
- StandardPredicateExpression

  Conforms when `Base` conforms to `StandardPredicateExpression`, `Other` conforms to `StandardPredicateExpression`, `Base.Output` conforms to `Collection`, `Other.Output` conforms to `Collection`, `Base.Output.Element` conforms to `Equatable`, and `Base.Output.Element` is `Other.Output.Element`.

