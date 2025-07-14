

- Create ML
- MLTextClassifier
-  MLTextClassifier.FeatureExtractorType 

Enumeration

# MLTextClassifier.FeatureExtractorType

The text feature extractor type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+visionOS 1.0+

``` source
enum FeatureExtractorType
```

## Topics

### Selecting a feature extractor type

case customEmbedding(URL)

A feature extractor that uses a custom embedding contained in a CoreML model file.

case staticEmbedding

A feature extractor that uses the standard, built-in word embeddings.

case bertEmbedding

A feature extractor that provides BERT contextual word embeddings.

case elmoEmbedding

A feature extractor that provides ELMo contextual word embeddings.

case dynamicEmbedding

A feature extractor that provides embeddings for words, based on their in-context use.

### Describing a feature extractor type

var description: String

A text representation of a feature extractor type.

var debugDescription: String

A text representation of the feature extractor type that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the feature extractor type shown in a playground.

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

### Selecting an algorithm type

case crf(revision: Int?)

A text classification algorithm that uses a statistical model of transition probabilities between words.

case maxEnt(revision: Int?)

A text classification algorithm that uses multinomial logistic regression based on the frequencies of words, independent of context.

case transferLearning(MLTextClassifier.FeatureExtractorType, revision: Int?)

A text classification algorithm that uses transfer learning by leveraging a feature extractor to generate embeddings.

