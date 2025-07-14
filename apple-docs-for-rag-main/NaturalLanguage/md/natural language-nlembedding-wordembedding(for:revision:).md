

- Natural Language
- NLEmbedding
-  wordEmbedding(for:revision:) 

Type Method

# wordEmbedding(for:revision:)

Retrieves a word embedding for a given language and revision.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class func wordEmbedding(
    for language: NLLanguage,
    revision: Int
) -> NLEmbedding?
```

## Parameters 

`language`  

The language of the word embedding, such as french.

`revision`  

The revision of the word embedding.

## Return Value

An NLEmbedding if available, otherwise `nil`.

## See Also

### Creating a word embedding

class func wordEmbedding(for: NLLanguage) -> NLEmbedding?

Retrieves a word embedding for a given language.

convenience init(contentsOf: URL) throws

Creates a word embedding from a model file.

