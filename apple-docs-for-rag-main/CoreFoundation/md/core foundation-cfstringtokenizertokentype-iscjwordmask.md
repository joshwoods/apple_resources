

- Core Foundation
- CFStringTokenizerTokenType
-  isCJWordMask 

Type Property

# isCJWordMask

Contains kana and/or ideographs.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static var isCJWordMask: CFStringTokenizerTokenType { get }
```

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

static var hasNonLettersMask: CFStringTokenizerTokenType

Contains punctuation, symbols, and so on.

