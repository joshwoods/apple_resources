

- Foundation
- PredicateExpressions
-  PredicateExpressions.DictionaryKeySubscript 

Structure

# PredicateExpressions.DictionaryKeySubscript

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct DictionaryKeySubscript where Wrapped : PredicateExpression, Key : PredicateExpression, Wrapped.Output == [Key.Output : Value], Key.Output : Hashable
```

## Topics

### Initializers

init(wrapped: Wrapped, key: Key)

### Instance Properties

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

  Conforms when `Wrapped` conforms to `StandardPredicateExpression`, `Key` conforms to `StandardPredicateExpression`, `Value` conforms to `Copyable`, `Value` conforms to `Escapable`, `Wrapped.Output` is `[Key.Output : Value]`, and `Key.Output` conforms to `Hashable`.

