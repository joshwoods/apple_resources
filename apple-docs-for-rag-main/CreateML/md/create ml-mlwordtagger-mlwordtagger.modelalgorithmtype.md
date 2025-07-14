

- Create ML
- MLWordTagger
-  MLWordTagger.ModelAlgorithmType 

Enumeration

# MLWordTagger.ModelAlgorithmType

The algorithm type.

macOS 10.14+

``` source
enum ModelAlgorithmType
```

## Topics

### Selecting an algorithm type

case crf(revision: Int?)

A conditional random field algorithm.

case transferLearning(MLWordTagger.FeatureExtractorType, revision: Int)

A transfer-learning algorithm.

enum FeatureExtractorType

The feature extractors that are available to train a word tagger using with the transfer-learning algorithm option.

### Describing an algorithm type

var description: String

A text representation of the model algorithm type.

var debugDescription: String

A text representation of the algorithm type that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the algorithm type in a playground.

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

init(validation: MLWordTagger.ModelParameters.ValidationData, algorithm: MLWordTagger.ModelAlgorithmType, language: NLLanguage?)

Creates model parameters.

enum ValidationData

The validation data.

