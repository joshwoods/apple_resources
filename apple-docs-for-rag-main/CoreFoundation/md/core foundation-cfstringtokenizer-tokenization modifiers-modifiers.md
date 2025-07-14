

- Core Foundation
- CFStringTokenizer
-  Tokenization Modifiers 

API Collection

# Tokenization Modifiers

Tokenization options are used with CFStringTokenizerCreate(_:_:_:_:_:) to specify how the string should be tokenized

## Overview

You use the tokenization unit options with CFStringTokenizerCreate(_:_:_:_:_:) to specify how a string should be tokenized.

You use the modifiers together with a tokenization unit to modify the way the string is tokenized.

You use the attribute specifiers to tell the tokenizer to prepare the specified attribute when it tokenizes the given string. You can retrieve the attribute value by calling CFStringTokenizerCopyCurrentTokenAttribute(_:_:) with one of the attribute options.

The locale sensitivity of the tokenization unit options may change in a future release.

## Topics

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

var kCFStringTokenizerAttributeLatinTranscription: CFOptionFlags

Used with `kCFStringTokenizerUnitWord`, tells the tokenizer to prepare the Latin transcription when it tokenizes the string.

var kCFStringTokenizerAttributeLanguage: CFOptionFlags

Tells the tokenizer to prepare the language (specified as an RFC 3066bis string) when it tokenizes the string.

## See Also

### Constants

struct CFStringTokenizerTokenType

Token types returned by CFStringTokenizerGoToTokenAtIndex(_:_:) and CFStringTokenizerAdvanceToNextToken(_:).

