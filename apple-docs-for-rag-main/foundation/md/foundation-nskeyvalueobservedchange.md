

- Foundation
-  NSKeyValueObservedChange 

Structure

# NSKeyValueObservedChange

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct NSKeyValueObservedChange
```

## Topics

### Instance Properties

let indexes: IndexSet?

indexes will be nil unless the observed KeyPath refers to an ordered to-many property

let isPrior: Bool

‘isPrior’ will be true if this change observation is being sent before the change happens, due to .prior being passed to `observe()`

let kind: NSKeyValueObservedChange&lt;Value>.Kind

let newValue: Value?

newValue and oldValue will only be non-nil if .new/.old is passed to `observe()`. In general, get the most up to date value by accessing it directly on the observed object instead.

let oldValue: Value?

### Type Aliases

typealias Kind

## Relationships

### Conforms To

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

struct NSKeyValueOperator

These constants define the available array operators. See Using Collection Operators for more information.

struct PresentationIntent

A type that defines presentation intent for blocks of characters like paragraphs, lists, block quotes, and tables.

