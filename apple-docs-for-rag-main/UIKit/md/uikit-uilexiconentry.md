

- UIKit
-  UILexiconEntry 

Class

# UILexiconEntry

A read-only term pair, available within a lexicon object, for a custom keyboard.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UILexiconEntry
```

## Overview

You can employ a lexicon entry by matching user input against the entry’s userInput value, and then inserting into the current text input object the corresponding documentText value. For example, if the user typed the string “iphone”, the lexicon entry with that exact, case-sensitive string in the userInput property has the string “iPhone” in the corresponding documentText property.

In some cases, the documentText string is in a different text script than the userInput string.

For information on custom keyboards, which are based on the UIInputViewController class, see Creating a custom keyboard.

## Topics

### Accessing a lexicon entry

var documentText: String

Text to be inserted into a text input object by a custom keyboard, corresponding to the user input value in the same lexicon entry.

var userInput: String

Text to match, during user input, to provide appropriate output to a text document from the document text value in the same lexicon entry.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable

## See Also

### Custom keyboard

protocol UITextDocumentProxy

An object that provides textual context to a custom keyboard.

protocol UIInputViewAudioFeedback

A property that enables a custom input or keyboard accessory view to play standard keyboard input clicks.

class UIInputViewController

The primary view controller for a custom keyboard app extension.

class UILexicon

A read-only array of term pairs, each in a lexicon entry object, for a custom keyboard.

