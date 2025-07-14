

- Natural Language
- NLEmbedding
-  currentSentenceEmbeddingRevision(for:) 

Type Method

# currentSentenceEmbeddingRevision(for:)

Retrieves the current version of a sentence embedding for the given language.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
class func currentSentenceEmbeddingRevision(for language: NLLanguage) -> Int
```

## Parameters 

`language`  

A language supported by the Natural Language framework. For possible values, see NLLanguage.

## Return Value

An integer representing the current version number of a sentence embedding.

## See Also

### Checking for Natural Language support

class func currentRevision(for: NLLanguage) -> Int

Retrieves the current version of a word embedding for the given language.

class func supportedRevisions(for: NLLanguage) -> IndexSet

Retrieves all version numbers of a word embedding for the given language.

class func supportedSentenceEmbeddingRevisions(for: NLLanguage) -> IndexSet

Retrieves all version numbers of a sentence embedding for the given language.

