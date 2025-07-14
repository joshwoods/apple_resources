

- Create ML
- MLTextClassifier
-  MLTextClassifier.ModelAlgorithmType 

Enumeration

# MLTextClassifier.ModelAlgorithmType

The type of algorithm that a text classifier uses.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+visionOS 1.0+

``` source
enum ModelAlgorithmType
```

## Mentioned in 

Improving Your Model’s Accuracy

Creating a text classifier model

## Overview

Typically, `maxEnt` is the fastest training algorithm. If the text classifier’s performance isn’t good enough, consider the `transferLearning` algorithm.

## Topics

### Selecting an algorithm type

case crf(revision: Int?)

A text classification algorithm that uses a statistical model of transition probabilities between words.

case maxEnt(revision: Int?)

A text classification algorithm that uses multinomial logistic regression based on the frequencies of words, independent of context.

case transferLearning(MLTextClassifier.FeatureExtractorType, revision: Int?)

A text classification algorithm that uses transfer learning by leveraging a feature extractor to generate embeddings.

enum FeatureExtractorType

The text feature extractor type.

### Describing an algorithm type

var description: String

A text representation of the algorithm type.

var debugDescription: String

A text representation of the algorithm type that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the algorithm type shown in a playground.

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
- Sendable

## See Also

### Creating parameters

init(validation: MLTextClassifier.ModelParameters.ValidationData, algorithm: MLTextClassifier.ModelAlgorithmType, language: NLLanguage?)

Creates model parameters for a text classifier with the specified validation data, algorithm, and language.

struct NLLanguage

The languages that the Natural Language framework supports.

enum ValidationData

The validation data that a text classifier uses.

