

- Core Foundation
- CFStringTokenizerTokenType
-  hasNonLettersMask 

Type Property

# hasNonLettersMask

Contains punctuation, symbols, and so on.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static var hasNonLettersMask: CFStringTokenizerTokenType { get }
```

## Discussion

Given the way Unicode word break works, this means it is a standalone punctuation or symbol character, or a string of such.

## See Also

### Constants

static var normal: CFStringTokenizerTokenType

Has a normal token.

static var hasSubTokensMask: CFStringTokenizerTokenType

Compound token which may contain subtokens but with no derived subtokens.

static var hasDerivedSubTokensMask: CFStringTokenizerTokenType

Compound token which may contain derived subtokens.

static var hasHasNumbersMask: CFStringTokenizerTokenType

Appears to contain a number.

static var isCJWordMask: CFStringTokenizerTokenType

Contains kana and/or ideographs.

