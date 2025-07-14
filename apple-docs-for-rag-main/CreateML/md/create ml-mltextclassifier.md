

- Create ML
-  MLTextClassifier 

Structure

# MLTextClassifier

A model you train to classify natural language text.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+visionOS 1.0+

``` source
struct MLTextClassifier
```

## Mentioned in 

Creating a Text Classifier Model

Creating a text classifier model

## Overview

Use a text classifier to train a machine learning model you can include in your app to classify natural language text. The model learns to associate labels with features of the input text, which can be sentences, paragraphs, or even entire documents.

After you train a text classifier, you save it to a Core ML model file. You then use an instance of the NLModel class from the Natural Language framework to read the model file into your app.

## Topics

### Creating and training a text classifier

init(trainingData: [String : [String]], parameters: MLTextClassifier.ModelParameters) throws

Creates a text classifier.

init(trainingData: DataFrame, textColumn: String, labelColumn: String, parameters: MLTextClassifier.ModelParameters) throws

Creates a text classifier.

init(trainingData: MLTextClassifier.DataSource, parameters: MLTextClassifier.ModelParameters) throws

Creates a text classifier.

enum DataSource

A data source for a text classifier.

struct ModelParameters

Parameters that specify model training parameters and validation data.

let modelParameters: MLTextClassifier.ModelParameters

The configuration parameters that the text classifier used for training during initialization.

init(trainingData: MLDataTable, textColumn: String, labelColumn: String, parameters: MLTextClassifier.ModelParameters) throws

Creates a text classifier.

Deprecated

### Assessing model accuracy

let trainingMetrics: MLClassifierMetrics

Measurements of the classifier’s performance on the training data set.

let validationMetrics: MLClassifierMetrics

Measurements of the classifier’s performance on the validation data set.

### Evaluating a text classifier

func evaluation(on: MLTextClassifier.DataSource) -> MLClassifierMetrics

Computes evaluation metrics.

func evaluation(on: DataFrame, textColumn: String, labelColumn: String) -> MLClassifierMetrics

Computes evaluation metrics.

func evaluation(on: [String : [String]]) -> MLClassifierMetrics

Computes evaluation metrics.

func evaluation(on: MLDataTable, textColumn: String, labelColumn: String) -> MLClassifierMetrics

Computes evaluation metrics.

Deprecated

### Testing a text classifier

func prediction(from: String) throws -> String

Classifies a string with a label.

func predictions(from: [String]) throws -> [String]

Classifies an array of strings with labels.

func predictionWithConfidence(from: String) throws -> [String : Double]

Predicts multiple possible labels and their confidence scores for the specified string.

func predictionsWithConfidence(from: [String]) throws -> [[String : Double]]

Predicts multiple possible labels and their confidence scores for each string in the specified array.

func predictions(from: MLDataColumn&lt;String>) throws -> MLDataColumn&lt;String>

Classifies a data column with labels.

Deprecated

func predictionsWithConfidence(from: MLDataColumn&lt;String>) throws -> MLDataColumn&lt;[String : Double]>

Predicts multiple possible labels and their confidence scores for each string in the specified data column.

Deprecated

### Saving a text classifier

func write(to: URL, metadata: MLModelMetadata?) throws

Exports the text classifier as a Core ML model file at the specified URL.

func write(toFile: String, metadata: MLModelMetadata?) throws

Exports the text classifier as a Core ML model file at the specified file path.

### Describing a text classifier

var model: MLModel

The underlying Core ML model of the text classifier.

var description: String

A text representation of the text classifier.

var debugDescription: String

A text representation of the text classifier that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the text classifier in a playground.

### Enumerations

enum FeatureExtractorType

The text feature extractor type.

enum ModelAlgorithmType

The type of algorithm that a text classifier uses.

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

### Text Models

Creating a text classifier model

Train a machine learning model to classify natural language text.

Creating a word tagger model

Train a machine learning model to tag individual words in natural language text.

struct MLWordTagger

A word-tagging model you train to classify natural language text at the word level.

struct MLGazetteer

A collection of terms and their labels, which augments a tagger that analyzes natural language text.

struct MLWordEmbedding

A map of strings in a vector space that enable your app to find similar strings by looking at a string’s neighbors.

