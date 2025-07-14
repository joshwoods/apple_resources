

- Create ML
- MLRecommender
- MLRecommender.ModelParameters
-  threshold 

Instance Property

# threshold

The item confidence value cutoff, below which the recommender omits those items from its recommendations.

macOS 10.15+

``` source
var threshold: Double
```

## Discussion

The default value is `0.001`.

## See Also

### Configuring the parameters

var algorithm: MLRecommender.ModelAlgorithmType

The algorithm the recommender uses to make recommendations.

var maxCount: Int

The largest number of similar items the model stores for each item.

var maxSimilarityIterations: Int

The largest number of iterations the recommender uses to build its lookup table.

var nearestItems: MLDataTable?

A data table that lists each item’s nearest items.

Deprecated

var nearestItemsDataFrame: DataFrame?

A data frame that lists each item’s nearest items.

