

- Foundation
-  Expression 

Structure

# Expression

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 1.0+watchOS 11.0+

``` source
struct Expression
```

## Topics

### Initializers

init((repeat PredicateExpressions.Variable&lt;each Input>) -> any StandardPredicateExpression&lt;Output>)

### Instance Properties

let expression: any StandardPredicateExpression&lt;Output>

let variable: (repeat PredicateExpressions.Variable&lt;each Input>)

### Instance Methods

func evaluate(repeat each Input) throws -> Output

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Decodable
- DecodableWithConfiguration

  Conforms when `each Input` conforms to `Copyable`, `each Input` conforms to `Escapable`, `Output` conforms to `Copyable`, and `Output` conforms to `Escapable`.

- Encodable
- EncodableWithConfiguration

  Conforms when `each Input` conforms to `Copyable`, `each Input` conforms to `Escapable`, `Output` conforms to `Copyable`, and `Output` conforms to `Escapable`.

- Sendable

## See Also

### Structures

struct AsyncCharacterSequence

An asynchronous sequence of characters.

struct AsyncLineSequence

An asynchronous sequence of lines of text.

struct AsyncUnicodeScalarSequence

An asychronous sequence of Unicode scalar values.

struct NSAttributedStringFormattingContextKey

struct NSKeyValueChangeKey

The keys that can appear in the change dictionary.

struct NSKeyValueObservedChange

struct NSKeyValueOperator

These constants define the available array operators. See Using Collection Operators for more information.

struct PresentationIntent

A type that defines presentation intent for blocks of characters like paragraphs, lists, block quotes, and tables.

