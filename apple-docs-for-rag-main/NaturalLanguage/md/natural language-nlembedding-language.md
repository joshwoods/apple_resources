

- Natural Language
- NLEmbedding
-  language 

Instance Property

# language

The language of the text in the word embedding.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var language: NLLanguage? { get }
```

## See Also

### Inspecting the vocabulary of an embedding

var dimension: Int

The number of dimensions in the vocabulary’s vector space.

var vocabularySize: Int

The number of words in the vocabulary.

func contains(String) -> Bool

Requests a Boolean value that indicates whether the term is in the vocabulary.

func vector(for: String) -> [Double]?

Requests the vector for the given term.

var revision: Int

The revision of the word embedding.

