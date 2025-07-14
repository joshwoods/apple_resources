

- Natural Language
- NLEmbedding
-  sentenceEmbedding(for:revision:) 

Type Method

# sentenceEmbedding(for:revision:)

Retrieves a sentence embedding for a given language and revision.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
class func sentenceEmbedding(
    for language: NLLanguage,
    revision: Int
) -> NLEmbedding?
```

## Parameters 

`language`  

The language of the sentence embedding, such as french. For possible values, see NLLanguage.

`revision`  

The revision of the sentence embedding.

## Return Value

An NLEmbedding if available, otherwise `nil`.

## See Also

### Creating a sentence embedding

class func sentenceEmbedding(for: NLLanguage) -> NLEmbedding?

Retrieves a sentence embedding for a given language.

