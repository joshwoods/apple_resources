

- Create ML
- MLRecommender
- MLRecommender.ModelParameters
-  algorithm 

Instance Property

# algorithm

The algorithm the recommender uses to make recommendations.

macOS 10.15+

``` source
var algorithm: MLRecommender.ModelAlgorithmType
```

## Discussion

The default is MLRecommender.ModelAlgorithmType.itemSimilarity(_:).

## See Also

### Configuring the parameters

var maxCount: Int

The largest number of similar items the model stores for each item.

var maxSimilarityIterations: Int

The largest number of iterations the recommender uses to build its lookup table.

var threshold: Double

The item confidence value cutoff, below which the recommender omits those items from its recommendations.

var nearestItems: MLDataTable?

A data table that lists each item’s nearest items.

Deprecated

var nearestItemsDataFrame: DataFrame?

A data frame that lists each item’s nearest items.

