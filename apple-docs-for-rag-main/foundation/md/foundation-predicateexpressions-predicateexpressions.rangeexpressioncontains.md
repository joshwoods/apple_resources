

- Foundation
- PredicateExpressions
-  PredicateExpressions.RangeExpressionContains 

Structure

# PredicateExpressions.RangeExpressionContains

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct RangeExpressionContains where RangeExpression : PredicateExpression, Element : PredicateExpression, RangeExpression.Output : RangeExpression, Element.Output == RangeExpression.Output.Bound
```

## Topics

### Initializers

init(range: RangeExpression, element: Element)

### Instance Properties

let element: Element

let range: RangeExpression

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- PredicateExpression
- Sendable
- StandardPredicateExpression

  Conforms when `RangeExpression` conforms to `StandardPredicateExpression`, `Element` conforms to `StandardPredicateExpression`, `RangeExpression.Output` conforms to `RangeExpression`, and `Element.Output` is `RangeExpression.Output.Bound`.

