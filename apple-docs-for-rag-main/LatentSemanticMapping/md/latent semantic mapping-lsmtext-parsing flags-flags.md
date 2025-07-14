

- Latent Semantic Mapping
- LSMText
-  Parsing Flags 

API Collection

# Parsing Flags

Options for parsing words to add to the text.

## Overview

Specify these options for LSMTextAddWords(_:_:_:_:).

## Topics

### Constants

var kLSMTextApplySpamHeuristics: Int

An option that specifies the parser should attempt to find words in hostile text.

var kLSMTextPreserveAcronyms: Int

An option that specifies the parser shouldn’t map all-uppercase words to lowercase.

var kLSMTextPreserveCase: Int

An option that specifies the parser shouldn’t change any words to lowercase.

## See Also

### Adding to the Text

func LSMTextAddToken(LSMText, CFData) -> OSStatus

Adds an arbitrary binary token to the text.

func LSMTextAddWord(LSMText, CFString) -> OSStatus

Adds a word to the text.

func LSMTextAddWords(LSMText, CFString, CFLocale?, CFOptionFlags) -> OSStatus

Breaks a string into words using the specified locale, and adds the words to the text.

