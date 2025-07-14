

- Create ML
- MLRecommender
-  MLRecommender.SimilarityType 

Enumeration

# MLRecommender.SimilarityType

The metric by which the recommender computes item similarity.

macOS 10.15+

``` source
enum SimilarityType
```

## Topics

### Similarity types

case jaccard

The Jaccard similarity measure.

case cosine

The cosine similarity measure.

case pearson

The Pearson correlation similarity measure.

### Comparing similarity types

static func == (MLRecommender.SimilarityType, MLRecommender.SimilarityType) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Getting the hash value

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

### Similarity type descriptions

var description: String

A text representation of the similarity type.

var debugDescription: String

A text representation of the similarity type that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the similarity type shown in a playground.

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

### Recommender algorithms

case itemSimilarity(MLRecommender.SimilarityType)

An algorithm that compares the similarity from item to item.

