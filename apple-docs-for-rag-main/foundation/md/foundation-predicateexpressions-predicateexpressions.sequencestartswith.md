

- Foundation
- PredicateExpressions
-  PredicateExpressions.SequenceStartsWith 

Structure

# PredicateExpressions.SequenceStartsWith

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct SequenceStartsWith where Base : PredicateExpression, Prefix : PredicateExpression, Base.Output : Sequence, Prefix.Output : Sequence, Base.Output.Element : Equatable, Base.Output.Element == Prefix.Output.Element
```

## Topics

### Initializers

init(base: Base, prefix: Prefix)

### Instance Properties

let base: Base

let prefix: Prefix

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- PredicateExpression
- Sendable
- StandardPredicateExpression

  Conforms when `Base` conforms to `StandardPredicateExpression`, `Prefix` conforms to `StandardPredicateExpression`, `Base.Output` conforms to `Sequence`, `Prefix.Output` conforms to `Sequence`, `Base.Output.Element` conforms to `Equatable`, and `Base.Output.Element` is `Prefix.Output.Element`.

