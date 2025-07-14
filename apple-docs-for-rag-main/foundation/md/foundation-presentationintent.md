

- Foundation
-  PresentationIntent 

Structure

# PresentationIntent

A type that defines presentation intent for blocks of characters like paragraphs, lists, block quotes, and tables.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct PresentationIntent
```

## Topics

### Structures

struct IntentType

struct TableColumn

### Initializers

init(PresentationIntent.Kind, identity: Int, parent: PresentationIntent?)

init(types: [PresentationIntent.IntentType])

### Instance Properties

var components: [PresentationIntent.IntentType]

var count: Int

var indentationLevel: Int

var isValid: Bool

### Enumerations

enum Kind

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Structures

struct AsyncCharacterSequence

An asynchronous sequence of characters.

struct AsyncLineSequence

An asynchronous sequence of lines of text.

struct AsyncUnicodeScalarSequence

An asychronous sequence of Unicode scalar values.

struct Expression

struct NSAttributedStringFormattingContextKey

struct NSKeyValueChangeKey

The keys that can appear in the change dictionary.

struct NSKeyValueObservedChange

struct NSKeyValueOperator

These constants define the available array operators. See Using Collection Operators for more information.

