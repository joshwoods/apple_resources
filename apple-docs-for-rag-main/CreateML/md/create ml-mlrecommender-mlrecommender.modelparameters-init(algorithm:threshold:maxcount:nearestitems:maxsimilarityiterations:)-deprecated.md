

- Create ML
- MLRecommender
- MLRecommender.ModelParameters
-  init(algorithm:threshold:maxCount:nearestItems:maxSimilarityIterations:) Deprecated

Initializer

# init(algorithm:threshold:maxCount:nearestItems:maxSimilarityIterations:)

Creates a new set of recommender configuration parameters.

macOS 10.15–14.0Deprecated

``` source
init(
    algorithm: MLRecommender.ModelAlgorithmType = .itemSimilarity(.cosine),
    threshold: Double = 0.001,
    maxCount: Int = 64,
    nearestItems: MLDataTable?,
    maxSimilarityIterations: Int = 1024
)
```

## See Also

### Creating parameters

init(algorithm: MLRecommender.ModelAlgorithmType, threshold: Double, maxCount: Int, nearestItemsDataFrame: DataFrame?, maxSimilarityIterations: Int)

Creates a new set of recommender configuration parameters.

enum ModelAlgorithmType

The algorithms a recommender can use to make recommendations.

