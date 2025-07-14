

- Core Foundation
-  kCFStringTokenizerAttributeLatinTranscription 

Global Variable

# kCFStringTokenizerAttributeLatinTranscription

Used with `kCFStringTokenizerUnitWord`, tells the tokenizer to prepare the Latin transcription when it tokenizes the string.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var kCFStringTokenizerAttributeLatinTranscription: CFOptionFlags { get }
```

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

var kCFStringTokenizerUnitWordBoundary: CFOptionFlags

Specifies that a string should be tokenized by locale-sensitive word boundary.

var kCFStringTokenizerAttributeLanguage: CFOptionFlags

Tells the tokenizer to prepare the language (specified as an RFC 3066bis string) when it tokenizes the string.

