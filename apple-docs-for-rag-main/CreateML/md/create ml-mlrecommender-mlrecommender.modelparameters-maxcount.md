

- Create ML
- MLRecommender
- MLRecommender.ModelParameters
-  maxCount 

Instance Property

# maxCount

The largest number of similar items the model stores for each item.

macOS 10.15+

``` source
var maxCount: Int
```

## Discussion

The memory Create ML requires to train this model is proportional to this number. A lower value reduces its demand for memory but decreases the recommender’s accuracy. The default value is `64`.

## See Also

### Configuring the parameters

var algorithm: MLRecommender.ModelAlgorithmType

The algorithm the recommender uses to make recommendations.

var maxSimilarityIterations: Int

The largest number of iterations the recommender uses to build its lookup table.

var threshold: Double

The item confidence value cutoff, below which the recommender omits those items from its recommendations.

var nearestItems: MLDataTable?

A data table that lists each item’s nearest items.

Deprecated

var nearestItemsDataFrame: DataFrame?

A data frame that lists each item’s nearest items.

