

- Core Foundation
-  CFStringTokenizerTokenType 

Structure

# CFStringTokenizerTokenType

Token types returned by CFStringTokenizerGoToTokenAtIndex(_:_:) and CFStringTokenizerAdvanceToNextToken(_:).

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CFStringTokenizerTokenType
```

## Overview

See http://www.unicode.org/reports/tr29/#Word_Boundaries for a detailed description of word boundaries.

## Topics

### Constants

static var normal: CFStringTokenizerTokenType

Has a normal token.

static var hasSubTokensMask: CFStringTokenizerTokenType

Compound token which may contain subtokens but with no derived subtokens.

static var hasDerivedSubTokensMask: CFStringTokenizerTokenType

Compound token which may contain derived subtokens.

static var hasHasNumbersMask: CFStringTokenizerTokenType

Appears to contain a number.

static var hasNonLettersMask: CFStringTokenizerTokenType

Contains punctuation, symbols, and so on.

static var isCJWordMask: CFStringTokenizerTokenType

Contains kana and/or ideographs.

### Initializers

init(rawValue: CFOptionFlags)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Constants

Tokenization Modifiers

Tokenization options are used with CFStringTokenizerCreate(_:_:_:_:_:) to specify how the string should be tokenized

