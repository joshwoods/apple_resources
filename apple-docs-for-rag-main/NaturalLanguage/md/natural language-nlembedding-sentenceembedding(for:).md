

- Natural Language
- NLEmbedding
-  sentenceEmbedding(for:) 

Type Method

# sentenceEmbedding(for:)

Retrieves a sentence embedding for a given language.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
class func sentenceEmbedding(for language: NLLanguage) -> NLEmbedding?
```

## Parameters 

`language`  

The language of the sentence embedding, such as french. For possible values, see NLLanguage.

## Return Value

An NLEmbedding if available, otherwise `nil`.

## Mentioned in 

Finding similarities between pieces of text

## See Also

### Creating a sentence embedding

class func sentenceEmbedding(for: NLLanguage, revision: Int) -> NLEmbedding?

Retrieves a sentence embedding for a given language and revision.

