

- Natural Language
- NLTokenUnit
-  NLTokenUnit.sentence 

Case

# NLTokenUnit.sentence

An individual sentence.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
case sentence
```

## Discussion

Use this linguistic unit to tokenize text into sentences, like in the following example:

```
let text = "This is a sentence. This is another sentence."

let tokenizer = NLTokenizer(unit: .sentence)
tokenizer.string = text

let range = text.startIndex..

For more information, see Tokenizing natural language text.

## See Also

### Constants

case word

An individual word.

case paragraph

An individual paragraph.

case document

The document in its entirety.

