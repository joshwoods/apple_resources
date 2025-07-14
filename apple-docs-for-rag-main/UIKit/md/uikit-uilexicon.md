

- UIKit
-  UILexicon 

Class

# UILexicon

A read-only array of term pairs, each in a lexicon entry object, for a custom keyboard.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UILexicon
```

## Mentioned in 

Configuring a custom keyboard interface

## Overview

To obtain the lexicon, call the requestSupplementaryLexicon(completion:) method of the UIInputViewController class. This method can be called only from a custom keyboard app extension. A lexicon contains words from various sources, including:

- Unpaired first names and last names from the user’s Address Book database

- Text shortcuts defined in the Settings \> General \> Keyboard \> Shortcuts list

- A common words dictionary

Apple intends for you to consider the words in a lexicon object as supplementary to an autocorrection/suggestion lexicon of your own design. For information on custom keyboards, see Custom Keyboard in App Extension Programming Guide.

## Topics

### Accessing the lexicon

var entries: [UILexiconEntry]

A read-only array of term pairs for use by a custom keyboard.

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

class UILexiconEntry

A read-only term pair, available within a lexicon object, for a custom keyboard.

