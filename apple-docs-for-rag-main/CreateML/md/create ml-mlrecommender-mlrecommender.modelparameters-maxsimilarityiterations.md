

- Create ML
- MLRecommender
- MLRecommender.ModelParameters
-  maxSimilarityIterations 

Instance Property

# maxSimilarityIterations

The largest number of iterations the recommender uses to build its lookup table.

macOS 10.15+

``` source
var maxSimilarityIterations: Int
```

## Discussion

This value limits the number of iterations the recommender can use to construct a lookup table. The default value is `1024`.

## See Also

### Configuring the parameters

var algorithm: MLRecommender.ModelAlgorithmType

The algorithm the recommender uses to make recommendations.

var maxCount: Int

The largest number of similar items the model stores for each item.

var threshold: Double

The item confidence value cutoff, below which the recommender omits those items from its recommendations.

var nearestItems: MLDataTable?

A data table that lists each item’s nearest items.

Deprecated

var nearestItemsDataFrame: DataFrame?

A data frame that lists each item’s nearest items.

