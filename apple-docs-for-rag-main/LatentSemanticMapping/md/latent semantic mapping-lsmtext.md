

- Latent Semantic Mapping
-  LSMText 

Class

# LSMText

An input text.

Mac CatalystmacOS

``` source
class LSMText
```

## Overview

An LSMText is a mutable, opaque Core Foundation type that represents an input text.

## Topics

### Creating a Text Object

func LSMTextCreate(CFAllocator?, LSMMap) -> Unmanaged&lt;LSMText>

Creates a new text.

### Adding to the Text

func LSMTextAddToken(LSMText, CFData) -> OSStatus

Adds an arbitrary binary token to the text.

func LSMTextAddWord(LSMText, CFString) -> OSStatus

Adds a word to the text.

func LSMTextAddWords(LSMText, CFString, CFLocale?, CFOptionFlags) -> OSStatus

Breaks a string into words using the specified locale, and adds the words to the text.

Parsing Flags

Options for parsing words to add to the text.

### Getting the Type Identifier

func LSMTextGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier for Latent Semantic Mapping texts.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Text Classification

class LSMMap

A map between a set of categories and related text.

class LSMResult

A result of a lookup in a map.

