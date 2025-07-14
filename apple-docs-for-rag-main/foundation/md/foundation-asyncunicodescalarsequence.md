

- Foundation
-  AsyncUnicodeScalarSequence 

Structure

# AsyncUnicodeScalarSequence

An asychronous sequence of Unicode scalar values.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct AsyncUnicodeScalarSequence where Base : AsyncSequence, Base.Element == UInt8
```

## Relationships

### Conforms To

- AsyncSequence
- Sendable

## See Also

### Structures

struct AsyncCharacterSequence

An asynchronous sequence of characters.

struct AsyncLineSequence

An asynchronous sequence of lines of text.

struct Expression

struct NSAttributedStringFormattingContextKey

struct NSKeyValueChangeKey

The keys that can appear in the change dictionary.

struct NSKeyValueObservedChange

struct NSKeyValueOperator

These constants define the available array operators. See Using Collection Operators for more information.

struct PresentationIntent

A type that defines presentation intent for blocks of characters like paragraphs, lists, block quotes, and tables.

