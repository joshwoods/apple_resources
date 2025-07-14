

- UIKit
- UITextInput
-  tokenizer 

Instance Property

# tokenizer

An input tokenizer that provides information about the granularity of text units.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
var tokenizer: any UITextInputTokenizer { get }
```

**Required**

## Discussion

Standard units of granularity include characters, words, lines, and paragraphs. In most cases, you may lazily create and assign an instance of a subclass of UITextInputStringTokenizer for this purpose. If you require different behavior than this system-provided tokenizer, you can create a custom tokenizer that adopts the UITextInputTokenizer protocol.

## See Also

### Tokenizing input text

protocol UITextInputTokenizer

A tokenizer, which is an object that allows the text input system to evaluate text units of different granularities.

