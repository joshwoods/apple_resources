

- Natural Language
- NLTokenUnit
-  NLTokenUnit.word 

Case

# NLTokenUnit.word

An individual word.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
case word
```

## Mentioned in 

Tokenizing natural language text

## Discussion

Use this linguistic unit to tokenize text into individual words, like in the following example:

```
let text = "This is a sentence containing several words. 😀"

let tokenizer = NLTokenizer(unit: .word)
tokenizer.string = text

let range = text.startIndex..

For more information, see Tokenizing natural language text.

## See Also

### Constants

case sentence

An individual sentence.

case paragraph

An individual paragraph.

case document

The document in its entirety.

