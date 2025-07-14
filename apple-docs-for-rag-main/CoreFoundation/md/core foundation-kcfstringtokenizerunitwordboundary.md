

- Core Foundation
-  kCFStringTokenizerUnitWordBoundary 

Global Variable

# kCFStringTokenizerUnitWordBoundary

Specifies that a string should be tokenized by locale-sensitive word boundary.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var kCFStringTokenizerUnitWordBoundary: CFOptionFlags { get }
```

## Discussion

You can use this constant in double-click range detection and whole word search. It is locale-sensitive. If the locale is `en_US_POSIX`, a colon (U+003A) is treated as a word separator. If the `locale` parameter of CFStringTokenizerCreate(_:_:_:_:_:) is `NULL`, the locale from the global `AppleTextBreakLocale` preference is used if it is available; otherwise the locale defaults to the first locale in `AppleLanguages`.

`kCFStringTokenizerUnitWordBoundary` also returns space between words as a token.

## See Also

### Constants

var kCFStringTokenizerUnitWord: CFOptionFlags

Specifies that a string should be tokenized by word. The `locale` parameter of CFStringTokenizerCreate(_:_:_:_:_:) is ignored.

var kCFStringTokenizerUnitSentence: CFOptionFlags

Specifies that a string should be tokenized by sentence. The `locale` parameter of CFStringTokenizerCreate(_:_:_:_:_:) is ignored.

var kCFStringTokenizerUnitParagraph: CFOptionFlags

Specifies that a string should be tokenized by paragraph. The `locale` parameter of CFStringTokenizerCreate(_:_:_:_:_:) is ignored.

var kCFStringTokenizerUnitLineBreak: CFOptionFlags

Specifies that a string should be tokenized by line break. The `locale` parameter of CFStringTokenizerCreate(_:_:_:_:_:) is ignored.

var kCFStringTokenizerAttributeLatinTranscription: CFOptionFlags

Used with `kCFStringTokenizerUnitWord`, tells the tokenizer to prepare the Latin transcription when it tokenizes the string.

var kCFStringTokenizerAttributeLanguage: CFOptionFlags

Tells the tokenizer to prepare the language (specified as an RFC 3066bis string) when it tokenizes the string.

