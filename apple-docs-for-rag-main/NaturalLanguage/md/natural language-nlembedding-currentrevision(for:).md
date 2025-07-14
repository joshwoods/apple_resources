

- Natural Language
- NLEmbedding
-  currentRevision(for:) 

Type Method

# currentRevision(for:)

Retrieves the current version of a word embedding for the given language.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class func currentRevision(for language: NLLanguage) -> Int
```

## Parameters 

`language`  

A language supported by the Natural Language framework.

## Return Value

An integer.

## See Also

### Checking for Natural Language support

class func supportedRevisions(for: NLLanguage) -> IndexSet

Retrieves all version numbers of a word embedding for the given language.

class func currentSentenceEmbeddingRevision(for: NLLanguage) -> Int

Retrieves the current version of a sentence embedding for the given language.

class func supportedSentenceEmbeddingRevisions(for: NLLanguage) -> IndexSet

Retrieves all version numbers of a sentence embedding for the given language.

