

- Create ML
- MLRecommender
- MLRecommender.ModelParameters
-  nearestItemsDataFrame 

Instance Property

# nearestItemsDataFrame

A data frame that lists each item’s nearest items.

macOS 14.0+

``` source
var nearestItemsDataFrame: DataFrame?
```

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

var nearestItems: MLDataTable?

A data table that lists each item’s nearest items.

Deprecated

