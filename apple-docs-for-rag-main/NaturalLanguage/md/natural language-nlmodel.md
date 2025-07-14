

- Natural Language
-  NLModel 

Class

# NLModel

A custom model trained to classify or tag natural language text.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
class NLModel
```

## Mentioned in 

Creating a word tagger model

## Overview

With Natural Language, you can create text classifier (MLTextClassifier) or word tagger (MLWordTagger) models. Use NLModel to integrate those models into your app. This integration ensures that your tokenization and tagger configurations are identical when you train your model and use it in your app.

If you create a text classifier as described in doc:creating-a-text-classifier-model, you can integrate that model into your app and use it to make predictions like this:

```
let text = "I am very happy."

do {
    let mlModel = try SentimentClassifier(configuration: MLModelConfiguration()).model

    let customModel = try NLModel(mlModel: mlModel)

    // Use the text classifier model to get the most likely label.
    if let label = customModel.predictedLabel(for: text) {
        print("Most likely label: \(label)")
    }

    // Get multiple possible labels with their associated confidence scores.
    let labelHypotheses = customModel.predictedLabelHypotheses(for: text, maximumCount: 3)
    print("Label confidence scores: \(labelHypotheses)")

} catch {
    print(error)
}
```

If you create a custom word tagger as described in Creating a word tagger model, you can integrate that model into your app and generate tags for new text input like this:

```
let text = "The iPad is my favorite Apple product."

do {
    let mlModel = try AppleTagger(configuration: MLModelConfiguration()).model

    let customModel = try NLModel(mlModel: mlModel)
    let customTagScheme = NLTagScheme("Apple")

    let tagger = NLTagger(tagSchemes: [.nameType, customTagScheme])
    tagger.string = text
    tagger.setModels([customModel], forTagScheme: customTagScheme)

    tagger.enumerateTags(in: text.startIndex..

## Topics

### Creating a model

convenience init(mlModel: MLModel) throws

Creates a new natural language model based on the given Core ML model instance.

convenience init(contentsOf: URL) throws

Creates a new natural language model based on a compiled Core ML model at the given URL.

### Making predictions

func predictedLabel(for: String) -> String?

Predicts a label for the given input string.

func predictedLabels(forTokens: [String]) -> [String]

Predicts a label for each string in the given array.

func predictedLabelHypotheses(for: String, maximumCount: Int) -> [String : Double]

Predicts multiple possible labels for the given input string.

func predictedLabelHypotheses(forTokens: [String], maximumCount: Int) -> [[String : Double]]

Predicts multiple possible labels for each string in the given array.

### Inspecting a model

var configuration: NLModelConfiguration

A configuration describing the natural language model.

class NLModelConfiguration

The configuration parameters of a natural language model.

### Related Documentation

struct MLTextClassifier

A model you train to classify natural language text.

struct MLWordTagger

A word-tagging model you train to classify natural language text at the word level.

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

### Natural language models

Creating a text classifier model

Train a machine learning model to classify natural language text.

Creating a word tagger model

Train a machine learning model to tag individual words in natural language text.

