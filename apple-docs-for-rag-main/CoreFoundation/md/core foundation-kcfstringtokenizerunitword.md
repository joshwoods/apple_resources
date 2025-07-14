

- Core Foundation
-  kCFStringTokenizerUnitWord 

Global Variable

# kCFStringTokenizerUnitWord

Specifies that a string should be tokenized by word. The `locale` parameter of CFStringTokenizerCreate(_:_:_:_:_:) is ignored.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var kCFStringTokenizerUnitWord: CFOptionFlags { get }
```

## See Also

### Constants

var kCFStringTokenizerUnitSentence: CFOptionFlags

Specifies that a string should be tokenized by sentence. The `locale` parameter of CFStringTokenizerCreate(_:_:_:_:_:) is ignored.

var kCFStringTokenizerUnitParagraph: CFOptionFlags

Specifies that a string should be tokenized by paragraph. The `locale` parameter of CFStringTokenizerCreate(_:_:_:_:_:) is ignored.

var kCFStringTokenizerUnitLineBreak: CFOptionFlags

Specifies that a string should be tokenized by line break. The `locale` parameter of CFStringTokenizerCreate(_:_:_:_:_:) is ignored.

var kCFStringTokenizerUnitWordBoundary: CFOptionFlags

Specifies that a string should be tokenized by locale-sensitive word boundary.

var kCFStringTokenizerAttributeLatinTranscription: CFOptionFlags

Used with `kCFStringTokenizerUnitWord`, tells the tokenizer to prepare the Latin transcription when it tokenizes the string.

var kCFStringTokenizerAttributeLanguage: CFOptionFlags

Tells the tokenizer to prepare the language (specified as an RFC 3066bis string) when it tokenizes the string.

