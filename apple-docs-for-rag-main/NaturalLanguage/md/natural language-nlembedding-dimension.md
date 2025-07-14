

- Natural Language
- NLEmbedding
-  dimension 

Instance Property

# dimension

The number of dimensions in the vocabulary’s vector space.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var dimension: Int { get }
```

## See Also

### Inspecting the vocabulary of an embedding

var vocabularySize: Int

The number of words in the vocabulary.

var language: NLLanguage?

The language of the text in the word embedding.

func contains(String) -> Bool

Requests a Boolean value that indicates whether the term is in the vocabulary.

func vector(for: String) -> [Double]?

Requests the vector for the given term.

var revision: Int

The revision of the word embedding.

