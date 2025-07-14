

- Natural Language
- NLEmbedding
-  contains(\_:) 

Instance Method

# contains(\_:)

Requests a Boolean value that indicates whether the term is in the vocabulary.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func contains(_ string: String) -> Bool
```

## Parameters 

`string`  

The term to search for in the word embedding.

## Return Value

`true` if the term is in the word embedding’s vocabulary, otherwise `false`.

## See Also

### Inspecting the vocabulary of an embedding

var dimension: Int

The number of dimensions in the vocabulary’s vector space.

var vocabularySize: Int

The number of words in the vocabulary.

var language: NLLanguage?

The language of the text in the word embedding.

func vector(for: String) -> [Double]?

Requests the vector for the given term.

var revision: Int

The revision of the word embedding.

