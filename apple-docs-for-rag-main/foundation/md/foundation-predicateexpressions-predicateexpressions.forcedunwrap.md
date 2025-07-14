

- Foundation
- PredicateExpressions
-  PredicateExpressions.ForcedUnwrap 

Structure

# PredicateExpressions.ForcedUnwrap

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct ForcedUnwrap where Inner : PredicateExpression, Inner.Output == Wrapped?
```

## Topics

### Initializers

init(Inner)

### Instance Properties

let inner: Inner

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- PredicateExpression
- Sendable
- StandardPredicateExpression

  Conforms when `Inner` conforms to `StandardPredicateExpression`, `Wrapped` conforms to `Copyable`, `Wrapped` conforms to `Escapable`, and `Inner.Output` is `Wrapped?`.

