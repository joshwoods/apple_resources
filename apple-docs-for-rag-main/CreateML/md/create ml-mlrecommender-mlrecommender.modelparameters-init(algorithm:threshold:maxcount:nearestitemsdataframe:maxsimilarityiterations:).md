

- Create ML
- MLRecommender
- MLRecommender.ModelParameters
-  init(algorithm:threshold:maxCount:nearestItemsDataFrame:maxSimilarityIterations:) 

Initializer

# init(algorithm:threshold:maxCount:nearestItemsDataFrame:maxSimilarityIterations:)

Creates a new set of recommender configuration parameters.

macOS 14.0+

``` source
init(
    algorithm: MLRecommender.ModelAlgorithmType = .itemSimilarity(.cosine),
    threshold: Double = 0.001,
    maxCount: Int = 64,
    nearestItemsDataFrame: DataFrame?,
    maxSimilarityIterations: Int = 1024
)
```

## See Also

### Creating parameters

init(algorithm: MLRecommender.ModelAlgorithmType, threshold: Double, maxCount: Int, nearestItems: MLDataTable?, maxSimilarityIterations: Int)

Creates a new set of recommender configuration parameters.

Deprecated

enum ModelAlgorithmType

The algorithms a recommender can use to make recommendations.

