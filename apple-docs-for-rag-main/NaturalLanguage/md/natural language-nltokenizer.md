

- Natural Language
-  NLTokenizer 

Class

# NLTokenizer

A tokenizer that segments natural language text into semantic units.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
class NLTokenizer
```

## Mentioned in 

Tokenizing natural language text

## Overview

NLTokenizer creates individual units from natural language text. Define the desired unit (word, sentence, paragraph, or document as declared in the NLTokenUnit) for tokenization, and then assign a string to tokenize. The enumerateTokensInRange:usingBlock: method provides the ranges of the tokens in the string based on the tokenization unit.

For more information, see Tokenizing natural language text.

Important

Use an NLTokenizer instance on one thread or one dispatch queue at a time. You do this by either serializing method calls to the tokenizer, or by creating a separate tokenizer instance for each thread and dispatch queue.

## Topics

### Creating a tokenizer

init(unit: NLTokenUnit)

Creates a tokenizer with the specified unit.

### Configuring a tokenizer

var string: String?

The text to be tokenized.

func setLanguage(NLLanguage)

Sets the language of the text to be tokenized.

var unit: NLTokenUnit

The linguistic unit that this tokenizer uses.

struct Attributes

Hints about the contents of the string for the tokenizer.

### Enumerating the tokens

func enumerateTokens(in: Range&lt;String.Index>, using: (Range&lt;String.Index>, NLTokenizer.Attributes) -> Bool)

Enumerates over a given range of the string and calls the specified block for each token.

func tokens(for: Range&lt;String.Index>) -> [Range&lt;String.Index>]

Tokenizes the string within the provided range.

func tokenRange(at: String.Index) -> Range&lt;String.Index>

Finds the range of the token at the given index.

func tokenRange(for: Range&lt;String.Index>) -> Range&lt;String.Index>

Finds the entire range of all tokens contained completely or partially within the specified range.

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

## See Also

### Tokenization

Tokenizing natural language text

Enumerate the words in a string.

