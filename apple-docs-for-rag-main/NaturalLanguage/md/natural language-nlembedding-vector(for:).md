

- Natural Language
- NLEmbedding
-  vector(for:) 

Instance Method

# vector(for:)

Requests the vector for the given term.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@nonobjc
func vector(for string: String) -> [Double]?
```

## Parameters 

`string`  

The term to find in the word embedding.

## Return Value

A vector represented as an array of doubles if present in the word embedding, otherwise `nil`.

## Mentioned in 

Finding similarities between pieces of text

## See Also

### Inspecting the vocabulary of an embedding

var dimension: Int

The number of dimensions in the vocabulary’s vector space.

var vocabularySize: Int

The number of words in the vocabulary.

var language: NLLanguage?

The language of the text in the word embedding.

func contains(String) -> Bool

Requests a Boolean value that indicates whether the term is in the vocabulary.

var revision: Int

The revision of the word embedding.

