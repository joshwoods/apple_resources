

- Foundation
- PredicateExpressions
-  PredicateExpressions.DictionaryKeyDefaultValueSubscript 

Structure

# PredicateExpressions.DictionaryKeyDefaultValueSubscript

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct DictionaryKeyDefaultValueSubscript where Wrapped : PredicateExpression, Key : PredicateExpression, Default : PredicateExpression, Wrapped.Output == [Key.Output : Default.Output], Key.Output : Hashable
```

## Topics

### Initializers

init(wrapped: Wrapped, key: Key, default: Default)

### Instance Properties

let `default`: Default

let key: Key

let wrapped: Wrapped

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- PredicateExpression
- Sendable
- StandardPredicateExpression

  Conforms when `Wrapped` conforms to `StandardPredicateExpression`, `Key` conforms to `StandardPredicateExpression`, `Default` conforms to `StandardPredicateExpression`, `Wrapped.Output` is `[Key.Output : Default.Output]`, and `Key.Output` conforms to `Hashable`.

