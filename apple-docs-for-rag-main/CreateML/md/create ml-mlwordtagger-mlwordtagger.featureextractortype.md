

- Create ML
- MLWordTagger
-  MLWordTagger.FeatureExtractorType 

Enumeration

# MLWordTagger.FeatureExtractorType

The feature extractors that are available to train a word tagger using with the transfer-learning algorithm option.

macOS 11.0+

``` source
enum FeatureExtractorType
```

## Topics

### Selecting a feature extractor type

case bertEmbedding

A feature extractor that provides BERT contextual word embeddings.

case elmoEmbedding

A feature extractor that provides ELMo contextual word embeddings.

case dynamicEmbedding

A feature extractor that provides embeddings for words, based on their in-context use.

Deprecated

### Describing a feature extractor type

var description: String

A text representation of a feature extractor type.

var debugDescription: String

A text representation of the feature extractor that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the feature extractor in a playground.

### Comparing feature extractors

static func == (MLWordTagger.FeatureExtractorType, MLWordTagger.FeatureExtractorType) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Accessing the hash value

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

### Default Implementations

CustomDebugStringConvertible Implementations

CustomPlaygroundDisplayConvertible Implementations

CustomStringConvertible Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomPlaygroundDisplayConvertible
- CustomStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Selecting an algorithm type

case crf(revision: Int?)

A conditional random field algorithm.

case transferLearning(MLWordTagger.FeatureExtractorType, revision: Int)

A transfer-learning algorithm.

