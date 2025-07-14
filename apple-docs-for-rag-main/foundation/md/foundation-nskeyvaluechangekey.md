

- Foundation
-  NSKeyValueChangeKey 

Structure

# NSKeyValueChangeKey

The keys that can appear in the change dictionary.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct NSKeyValueChangeKey
```

## Discussion

These constants are used as keys in the change dictionary passed to observeValue(forKeyPath:of:change:context:).

## Topics

### Type Properties

static let indexesKey: NSKeyValueChangeKey

If the value of the kindKey entry is NSKeyValueChange.insertion, NSKeyValueChange.removal, or NSKeyValueChange.replacement, the value of this key is an `NSIndexSet` object that contains the indexes of the inserted, removed, or replaced objects.

static let kindKey: NSKeyValueChangeKey

An `NSNumber` object that contains a value corresponding to one of the NSKeyValueChange enums, indicating what sort of change has occurred.

static let newKey: NSKeyValueChangeKey

If the value of the kindKey entry is NSKeyValueChange.setting, and new was specified when the observer was registered, the value of this key is the new value for the attribute.

static let notificationIsPriorKey: NSKeyValueChangeKey

If the prior option was specified when the observer was registered this notification is sent prior to a change.

static let oldKey: NSKeyValueChangeKey

If the value of the kindKey entry is NSKeyValueChange.setting, and old was specified when the observer was registered, the value of this key is the value before the attribute was changed.

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
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

struct NSKeyValueObservedChange

struct NSKeyValueOperator

These constants define the available array operators. See Using Collection Operators for more information.

struct PresentationIntent

A type that defines presentation intent for blocks of characters like paragraphs, lists, block quotes, and tables.

