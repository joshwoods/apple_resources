

- Core Foundation
-  CFStringTokenizer 

Class

# CFStringTokenizer

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CFStringTokenizer
```

## Overview

CFStringTokenizer allows you to tokenize strings into words, sentences or paragraphs in a language-neutral way. It supports languages such as Japanese and Chinese that do not delimit words by spaces, as well as de-compounding German compounds. You can obtain Latin transcription for tokens. It also provides language identification API.

You can use a CFStringTokenizer to break a string into tokens (sub-strings) on the basis of words, sentences, or paragraphs. When you create a tokenizer, you can supply options to further modify the tokenization—see Tokenization Modifiers.

In addition, with CFStringTokenizer:

- You can de-compound German compounds

- You can identify the language used in a string (using CFStringTokenizerCopyBestStringLanguage(_:_:))

- You can obtain Latin transcription for tokens

To find a token that includes the character specified by character index and set it as the current token, you call CFStringTokenizerGoToTokenAtIndex(_:_:). To advance to the next token and set it as the current token, you call CFStringTokenizerAdvanceToNextToken(_:). To get the range of current token, you call CFStringTokenizerGetCurrentTokenRange(_:). You can use CFStringTokenizerCopyCurrentTokenAttribute(_:_:) to get the attribute of the current token. If the current token is a compound, you can call CFStringTokenizerGetCurrentSubTokens(_:_:_:_:) to retrieve the subtokens or derived subtokens contained in the compound token. To guess the language of a string, you call CFStringTokenizerCopyBestStringLanguage(_:_:).

## Topics

### Creating a Tokenizer

func CFStringTokenizerCreate(CFAllocator!, CFString!, CFRange, CFOptionFlags, CFLocale!) -> CFStringTokenizer!

Returns a tokenizer for a given string.

### Setting the String

func CFStringTokenizerSetString(CFStringTokenizer!, CFString!, CFRange)

Sets the string for a tokenizer.

### Changing the Location

func CFStringTokenizerAdvanceToNextToken(CFStringTokenizer!) -> CFStringTokenizerTokenType

Advances the tokenizer to the next token and sets that as the current token.

func CFStringTokenizerGoToTokenAtIndex(CFStringTokenizer!, CFIndex) -> CFStringTokenizerTokenType

Finds a token that includes the character at a given index, and set it as the current token.

### Getting Information About the Current Token

func CFStringTokenizerCopyCurrentTokenAttribute(CFStringTokenizer!, CFOptionFlags) -> CFTypeRef!

Returns a given attribute of the current token.

func CFStringTokenizerGetCurrentTokenRange(CFStringTokenizer!) -> CFRange

Returns the range of the current token.

func CFStringTokenizerGetCurrentSubTokens(CFStringTokenizer!, UnsafeMutablePointer&lt;CFRange>!, CFIndex, CFMutableArray!) -> CFIndex

Retrieves the subtokens or derived subtokens contained in the compound token.

### Identifying a Language

func CFStringTokenizerCopyBestStringLanguage(CFString!, CFRange) -> CFString!

Guesses a language of a given string and returns the guess as a BCP 47 string.

### Getting the CFStringTokenizer Type ID

func CFStringTokenizerGetTypeID() -> CFTypeID

Returns the type ID for CFStringTokenizer.

### Constants

Tokenization Modifiers

Tokenization options are used with CFStringTokenizerCreate(_:_:_:_:_:) to specify how the string should be tokenized

struct CFStringTokenizerTokenType

Token types returned by CFStringTokenizerGoToTokenAtIndex(_:_:) and CFStringTokenizerAdvanceToNextToken(_:).

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Related Documentation

String Programming Guide for Core Foundation

### Opaque Types

class CFAllocator

class CFArray

class CFAttributedString

class CFBag

class CFBinaryHeap

class CFBitVector

class CFBoolean

class CFBundle

class CFCalendar

class CFCharacterSet

class CFData

class CFDate

class CFDateFormatter

class CFDictionary

class CFError

