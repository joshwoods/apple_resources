

- Create ML
-  MLWordEmbedding 

Structure

# MLWordEmbedding

A map of strings in a vector space that enable your app to find similar strings by looking at a string’s neighbors.

macOS 10.15+

``` source
struct MLWordEmbedding
```

## Overview

Use an MLWordEmbedding to configure and save a word embedding to a file, which you then add to your project in Xcode. Your project uses that word embedding file at runtime to create an NLEmbedding instance, which finds similar strings based on the proximity of their vectors.

You configure a word embedding with a dictionary, keyed by strings which make up the *vocabulary* of the word embedding. The value for each string is an array of doubles, which represents a vector. The length of the arrays is arbitrary but all arrays in a word embedding must be the same length. The length of the arrays determine the number of dimensions in the vector space. For example, the following listing creates a word embedding with four dimensions and a vocabulary of two strings.

```
let wordEmbedding = try! MLWordEmbedding(dictionary: [
    "Hello"   : [0.0, 1.2, 5.0, 0.0],
    "Goodbye" : [0.0, 1.3, -6.2, 0.1]
])
```

Once you’ve configured an MLWordEmbedding, save it to an `.mlmodel` file to include in your app.

```
try wordEmbedding.write(toFile: "~/Desktop/WordEmbedding.mlmodel")
```

A word embedding file can efficiently store many strings and their vectors.

## Topics

### Creating a word embedding

init(dictionary: [String : [Double]], parameters: MLWordEmbedding.ModelParameters) throws

Creates a word embedding.

struct ModelParameters

The model configuration parameters.

let modelParameters: MLWordEmbedding.ModelParameters

The model configuration parameters.

### Testing a word embedding

func prediction(from: String, maxCount: Int, maxDistance: Double, distanceType: NLDistanceType) throws -> [(text: String, distance: Double)]

Predicts neighbors.

func distance(between: String, and: String, distanceType: NLDistanceType) -> Double

Calculates the distance between two strings in the vocabulary space.

enum NLDistanceType

The means of calculating a distance between two locations in a text embedding.

func contains(String) -> Bool

Returns a Boolean value indicating whether the vocabulary contains the given string.

func vector(for: String) -> [Double]?

Accesses the vector associated with the given string in the vocabulary.

### Saving a word embedding

func write(to: URL, metadata: MLModelMetadata?) throws

Exports the word embedding as a Core ML model file at the specified URL.

func write(toFile: String, metadata: MLModelMetadata?) throws

Exports the word embedding as a Core ML model file at the specified file path.

### Describing a word embedding

let dimension: Int

The number of dimensions in the vocabulary embedding space.

let vocabularySize: Int

The number of strings in the vocabulary.

var model: MLModel

The word embedding contained within a Core ML model file.

var description: String

A text representation of the word embedding.

var debugDescription: String

A text representation of the word embedding that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the word embedding shown in a playground.

### Default Implementations

CustomDebugStringConvertible Implementations

CustomPlaygroundDisplayConvertible Implementations

CustomStringConvertible Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomPlaygroundDisplayConvertible
- CustomStringConvertible

## See Also

### Text Models

Creating a text classifier model

Train a machine learning model to classify natural language text.

Creating a word tagger model

Train a machine learning model to tag individual words in natural language text.

struct MLTextClassifier

A model you train to classify natural language text.

struct MLWordTagger

A word-tagging model you train to classify natural language text at the word level.

struct MLGazetteer

A collection of terms and their labels, which augments a tagger that analyzes natural language text.

