

- Natural Language
- NLEmbedding
-  wordEmbedding(for:) 

Type Method

# wordEmbedding(for:)

Retrieves a word embedding for a given language.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class func wordEmbedding(for language: NLLanguage) -> NLEmbedding?
```

## Parameters 

`language`  

The language of the word embedding, such as french.

## Return Value

An NLEmbedding if available, otherwise `nil`.

## Mentioned in 

Finding similarities between pieces of text

## See Also

### Creating a word embedding

class func wordEmbedding(for: NLLanguage, revision: Int) -> NLEmbedding?

Retrieves a word embedding for a given language and revision.

convenience init(contentsOf: URL) throws

Creates a word embedding from a model file.

