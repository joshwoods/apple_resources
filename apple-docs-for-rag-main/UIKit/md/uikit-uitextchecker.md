

- UIKit
-  UITextChecker 

Class

# UITextChecker

An object to check a string (usually the text of a document) for misspelled words.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UITextChecker
```

## Overview

UITextChecker spell-checks using a lexicon for a specific language. You can tell it to ignore specific words when spell-checking a particular document and you can have it learn words, which adds those words to the lexicon. You generally use one instance of UITextChecker per document, although you can use a single instance to spell-check related pieces of text if you want to share ignored words and other state.

You may also use a text checker to obtain completions for partially entered words, as well as possible replacements for misspelled words, which you then can present to users.

## Topics

### Initiating a Spell Check

func rangeOfMisspelledWord(in: String, range: NSRange, startingAt: Int, wrap: Bool, language: String) -> NSRange

Initiates a search of a range of a string for a misspelled word.

### Obtaining Word Guesses and Completions

func guesses(forWordRange: NSRange, in: String, language: String) -> [String]?

Returns a list of words that are possible valid replacements for a misspelled word.

func completions(forPartialWordRange: NSRange, in: String, language: String) -> [String]?

Returns an array of strings that are possible completions for a partially entered word.

### Learning and Ignoring Words

func ignoreWord(String)

Tells the text checker to ignore the specified word when spell-checking.

var ignoredWords: [String]?

Returns the words that the text checker ignores when spell-checking.

class func learnWord(String)

Tells the text checker to learn the specified word so that it doesn’t evaluate it as misspelled.

class func unlearnWord(String)

Tells the text checker to unlearn the specified word.

class func hasLearnedWord(String) -> Bool

Returns whether the text checker has learned the specified word.

### Getting the Available Languages

class var availableLanguages: [String]

Returns the languages that the text checker’s class can perform spell-checking for.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

