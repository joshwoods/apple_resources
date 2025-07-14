

- Natural Language
- NLTokenUnit
-  NLTokenUnit.paragraph 

Case

# NLTokenUnit.paragraph

An individual paragraph.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
case paragraph
```

## Discussion

Use this linguistic unit to tokenize text into paragraphs, like in the following example:

```
let text = "This is a sentence. This is another sentence.\nThis is a second paragraph."

let tokenizer = NLTokenizer(unit: .paragraph)
tokenizer.string = text

let range = text.startIndex..

For more information, see Tokenizing natural language text.

## See Also

### Constants

case word

An individual word.

case sentence

An individual sentence.

case document

The document in its entirety.

