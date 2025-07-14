

- Natural Language
-  NLEmbedding 

Class

# NLEmbedding

A map of strings to vectors, which locates neighboring, similar strings.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class NLEmbedding
```

## Mentioned in 

Finding similarities between pieces of text

## Overview

Use an NLEmbedding to find similar strings based on the proximity of their vectors. The *vocabulary* is the entire set of strings in an embedding. Each string in the vocabulary has a vector, which is an array of doubles, and each double corresponds to a dimension in the embedding. An NLEmbedding uses these vectors to determine the distance between two strings, or to find the nearest neighbors of a string in the vocabulary. The higher the similarity of any two strings, the smaller the distance is between them.

Natural Language provides built-in word embeddings that you can retrieve by using the wordEmbedding(for:) method. You can also compile your own custom embedding into an efficient, searchable, on-disk representation. Typically, you compile an embedding by using Create ML’s MLWordEmbedding and save it as a file for your Xcode project at development time. Alternatively, you can compile an embedding at runtime by using Natural Language’s writeEmbeddingForDictionary:language:revision:toURL:error: method.

Your custom embedding can use any kind of string that’s useful to your app, such as phrases, brand names, serial numbers, and so on. For example, you could make an embedding of movie titles. Each movie title could have a vector that places similar movies close together in the embedding.

## Topics

### Creating a word embedding

class func wordEmbedding(for: NLLanguage) -> NLEmbedding?

Retrieves a word embedding for a given language.

class func wordEmbedding(for: NLLanguage, revision: Int) -> NLEmbedding?

Retrieves a word embedding for a given language and revision.

convenience init(contentsOf: URL) throws

Creates a word embedding from a model file.

### Creating a sentence embedding

class func sentenceEmbedding(for: NLLanguage) -> NLEmbedding?

Retrieves a sentence embedding for a given language.

class func sentenceEmbedding(for: NLLanguage, revision: Int) -> NLEmbedding?

Retrieves a sentence embedding for a given language and revision.

### Finding strings and their distances in an embedding

func neighbors(for: String, maximumCount: Int, distanceType: NLDistanceType) -> [(String, NLDistance)]

Retrieves a limited number of strings near a string in the vocabulary.

func neighbors(for: [Double], maximumCount: Int, distanceType: NLDistanceType) -> [(String, NLDistance)]

Retrieves a limited number of strings near a location in the vocabulary space.

func enumerateNeighbors(for: String, maximumCount: Int, distanceType: NLDistanceType, using: (String, NLDistance) -> Bool)

Passes the nearest strings of a string in the vocabulary to a closure.

func enumerateNeighbors(for: [Double], maximumCount: Int, distanceType: NLDistanceType, using: (String, NLDistance) -> Bool)

Passes the nearest strings of a location in the vocabulary space to a closure.

func distance(between: String, and: String, distanceType: NLDistanceType) -> NLDistance

Calculates the distance between two strings in the vocabulary space.

typealias NLDistance

The distance between two strings in a text embedding.

### Inspecting the vocabulary of an embedding

var dimension: Int

The number of dimensions in the vocabulary’s vector space.

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

### Saving an embedding

class func write([String : [Double]], language: NLLanguage?, revision: Int, to: URL) throws

Exports the word embedding contained within a Core ML model file at the given URL.

### Checking for Natural Language support

class func currentRevision(for: NLLanguage) -> Int

Retrieves the current version of a word embedding for the given language.

class func supportedRevisions(for: NLLanguage) -> IndexSet

Retrieves all version numbers of a word embedding for the given language.

class func currentSentenceEmbeddingRevision(for: NLLanguage) -> Int

Retrieves the current version of a sentence embedding for the given language.

class func supportedSentenceEmbeddingRevisions(for: NLLanguage) -> IndexSet

Retrieves all version numbers of a sentence embedding for the given language.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Text embedding

Finding similarities between pieces of text

Calculate the semantic distance between words or sentences.

