

- Create ML
- MLRecommender
-  MLRecommender.ModelAlgorithmType 

Enumeration

# MLRecommender.ModelAlgorithmType

The algorithms a recommender can use to make recommendations.

macOS 10.15+

``` source
enum ModelAlgorithmType
```

## Topics

### Recommender algorithms

case itemSimilarity(MLRecommender.SimilarityType)

An algorithm that compares the similarity from item to item.

enum SimilarityType

The metric by which the recommender computes item similarity.

### Algorithm descriptions

var description: String

A text representation of the recommender algorithm.

var debugDescription: String

A text representation of the recommender algorithm that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the recommender algorithm shown in a playground.

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

init(algorithm: MLRecommender.ModelAlgorithmType, threshold: Double, maxCount: Int, nearestItemsDataFrame: DataFrame?, maxSimilarityIterations: Int)

Creates a new set of recommender configuration parameters.

init(algorithm: MLRecommender.ModelAlgorithmType, threshold: Double, maxCount: Int, nearestItems: MLDataTable?, maxSimilarityIterations: Int)

Creates a new set of recommender configuration parameters.

Deprecated

