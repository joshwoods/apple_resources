

- Natural Language
- NLEmbedding
-  supportedSentenceEmbeddingRevisions(for:) 

Type Method

# supportedSentenceEmbeddingRevisions(for:)

Retrieves all version numbers of a sentence embedding for the given language.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
class func supportedSentenceEmbeddingRevisions(for language: NLLanguage) -> IndexSet
```

## Parameters 

`language`  

A language supported by the Natural Language framework. For possible values, see NLLanguage.

## Return Value

An index set representing all of the supported version numbers of the sentence embedding.

## See Also

### Checking for Natural Language support

class func currentRevision(for: NLLanguage) -> Int

Retrieves the current version of a word embedding for the given language.

class func supportedRevisions(for: NLLanguage) -> IndexSet

Retrieves all version numbers of a word embedding for the given language.

class func currentSentenceEmbeddingRevision(for: NLLanguage) -> Int

Retrieves the current version of a sentence embedding for the given language.

