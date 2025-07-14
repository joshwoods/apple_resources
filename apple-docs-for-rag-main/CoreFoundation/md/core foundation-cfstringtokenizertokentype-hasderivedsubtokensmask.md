

- Core Foundation
- CFStringTokenizerTokenType
-  hasDerivedSubTokensMask 

Type Property

# hasDerivedSubTokensMask

Compound token which may contain derived subtokens.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static var hasDerivedSubTokensMask: CFStringTokenizerTokenType { get }
```

## Discussion

You can obtain subtokens and derived subtokens by calling CFStringTokenizerGetCurrentSubTokens(_:_:_:_:).

## See Also

### Constants

static var normal: CFStringTokenizerTokenType

Has a normal token.

static var hasSubTokensMask: CFStringTokenizerTokenType

Compound token which may contain subtokens but with no derived subtokens.

static var hasHasNumbersMask: CFStringTokenizerTokenType

Appears to contain a number.

static var hasNonLettersMask: CFStringTokenizerTokenType

Contains punctuation, symbols, and so on.

static var isCJWordMask: CFStringTokenizerTokenType

Contains kana and/or ideographs.

