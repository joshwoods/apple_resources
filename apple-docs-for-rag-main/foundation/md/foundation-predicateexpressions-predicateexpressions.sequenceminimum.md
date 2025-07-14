

- Foundation
- PredicateExpressions
-  PredicateExpressions.SequenceMinimum 

Structure

# PredicateExpressions.SequenceMinimum

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct SequenceMinimum where Elements : PredicateExpression, Elements.Output : Sequence, Elements.Output.Element : Comparable
```

## Topics

### Initializers

init(elements: Elements)

### Instance Properties

let elements: Elements

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- PredicateExpression
- Sendable
- StandardPredicateExpression

  Conforms when `Elements` conforms to `StandardPredicateExpression`, `Elements.Output` conforms to `Sequence`, and `Elements.Output.Element` conforms to `Comparable`.

