

- Foundation
- PredicateExpressions
-  PredicateExpressions.StringLocalizedStandardContains 

Structure

# PredicateExpressions.StringLocalizedStandardContains

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct StringLocalizedStandardContains where Root : PredicateExpression, Other : PredicateExpression, Root.Output : StringProtocol, Other.Output : StringProtocol
```

## Topics

### Initializers

init(root: Root, other: Other)

### Instance Properties

let other: Other

let root: Root

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- PredicateExpression
- Sendable
- StandardPredicateExpression

  Conforms when `Root` conforms to `StandardPredicateExpression`, `Other` conforms to `StandardPredicateExpression`, `Root.Output` conforms to `StringProtocol`, and `Other.Output` conforms to `StringProtocol`.

