

- Create ML
- MLRecommender
- MLRecommender.ModelParameters
-  nearestItems Deprecated

Instance Property

# nearestItems

A data table that lists each item’s nearest items.

macOS 10.15–14.0Deprecated

``` source
var nearestItems: MLDataTable?
```

Deprecated

Use nearestItemsDataFrame.

## See Also

### Configuring the parameters

var algorithm: MLRecommender.ModelAlgorithmType

The algorithm the recommender uses to make recommendations.

var maxCount: Int

The largest number of similar items the model stores for each item.

var maxSimilarityIterations: Int

The largest number of iterations the recommender uses to build its lookup table.

var threshold: Double

The item confidence value cutoff, below which the recommender omits those items from its recommendations.

var nearestItemsDataFrame: DataFrame?

A data frame that lists each item’s nearest items.

