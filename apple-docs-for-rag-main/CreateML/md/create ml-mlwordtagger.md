

- Create ML
-  MLWordTagger 

Structure

# MLWordTagger

A word-tagging model you train to classify natural language text at the word level.

macOS 10.14+

``` source
struct MLWordTagger
```

## Overview

Use an MLWordTagger to create a custom word tagger to identify content that’s relevant for your app, like product names and points of interest.

To use your custom word tagger in the Natural Language framework, save it to a model file and import it into an NLModel. Then add your custom NLModel to an NLTagger with its setModels(_:forTagScheme:) method.

## Topics

### Creating and training a word tagger

init(trainingData: [(tokens: [MLWordTagger.Token], labels: [String])], parameters: MLWordTagger.ModelParameters) throws

Creates a word tagger.

init(trainingData: MLDataTable, tokenColumn: String, labelColumn: String, parameters: MLWordTagger.ModelParameters) throws

Creates a word tagger.

Deprecated

init(trainingData: DataFrame, tokenColumn: String, labelColumn: String, parameters: MLWordTagger.ModelParameters) throws

Creates a word tagger.

typealias Token

The token type of a word tagger, which is a string.

struct ModelParameters

Parameters that specify model training parameters and validation data.

let modelParameters: MLWordTagger.ModelParameters

The configuration parameters that the word tagger used for training during initialization.

### Assessing model accuracy

let trainingMetrics: MLWordTaggerMetrics

Measurements of the tagger’s performance on the training data set.

let validationMetrics: MLWordTaggerMetrics

Measurements of the tagger’s performance on the validation data set.

struct MLWordTaggerMetrics

Metrics you use to evaluate a word tagger’s performance.

### Evaluating a word tagger

func evaluation(on: MLDataTable, tokenColumn: String, labelColumn: String) -> MLWordTaggerMetrics

Computes evaluation metrics.

Deprecated

func evaluation(on: DataFrame, tokenColumn: String, labelColumn: String) -> MLWordTaggerMetrics

Computes evaluation metrics.

func evaluation(on: [(tokens: [MLWordTagger.Token], labels: [String])]) -> MLWordTaggerMetrics

Computes evaluation metrics.

### Testing a word tagger

func predictions&lt;S>(from: S) throws -> DataFrame

Predicts sequences of labels, token locations, and token lengths from the input strings.

func predictions(from: MLDataColumn&lt;String>) throws -> MLDataTable

Predicts sequences of labels, token locations, and token lengths from the input column containing strings.

Deprecated

func prediction(from: [MLWordTagger.Token]) throws -> [String]

Predicts a tag for each token in the specified array.

func prediction(from: String) throws -> [String]

Predicts a tag for the input string.

func predictionWithConfidence(from: String) throws -> [[String : Double]]

Predicts tags and confidence scores for the input string. Predicts tags and confidence scores for the input string.

func predictionWithConfidence(from: [MLWordTagger.Token]) throws -> [[String : Double]]

Predicts tags and confidence scores for each token in the specified token array.

### Saving a word tagger

func write(to: URL, metadata: MLModelMetadata?) throws

Exports the word tagger as a Core ML model file at the specified URL.

func write(toFile: String, metadata: MLModelMetadata?) throws

Exports the word tagger as a Core ML model file at the specified file path.

### Describing a word tagger

var model: MLModel

The underlying Core ML model of the word tagger.

var description: String

A text representation of the word tagger.

var debugDescription: String

A text representation of the word tagger that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the word tagger in a playground.

### Enumerations

enum FeatureExtractorType

The feature extractors that are available to train a word tagger using with the transfer-learning algorithm option.

enum ModelAlgorithmType

The algorithm type.

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

struct MLTextClassifier

A model you train to classify natural language text.

struct MLGazetteer

A collection of terms and their labels, which augments a tagger that analyzes natural language text.

struct MLWordEmbedding

A map of strings in a vector space that enable your app to find similar strings by looking at a string’s neighbors.

