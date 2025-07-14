

- Create ML
- MLRecommender
-  MLRecommender.ModelParameters 

Structure

# MLRecommender.ModelParameters

Parameters that affect the process of training a recommender model.

macOS 10.15+

``` source
struct ModelParameters
```

## Topics

### Creating parameters

init(algorithm: MLRecommender.ModelAlgorithmType, threshold: Double, maxCount: Int, nearestItemsDataFrame: DataFrame?, maxSimilarityIterations: Int)

Creates a new set of recommender configuration parameters.

init(algorithm: MLRecommender.ModelAlgorithmType, threshold: Double, maxCount: Int, nearestItems: MLDataTable?, maxSimilarityIterations: Int)

Creates a new set of recommender configuration parameters.

Deprecated

enum ModelAlgorithmType

The algorithms a recommender can use to make recommendations.

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

var nearestItemsDataFrame: DataFrame?

A data frame that lists each item’s nearest items.

## See Also

### Creating and training a recommender

init(trainingData: DataFrame, userColumn: String, itemColumn: String, ratingColumn: String?, parameters: MLRecommender.ModelParameters) throws

Creates an instance given a table and the names of the item and user columns contained therein.

init(trainingData: MLDataTable, userColumn: String, itemColumn: String, ratingColumn: String?, parameters: MLRecommender.ModelParameters) throws

Creates an instance given a table and the names of the item and user columns contained therein.

Deprecated

let modelParameters: MLRecommender.ModelParameters

The configuration parameters that the recommender used for training during initialization.

var userIdentifierColumn: String

The name of the column you selected at initialization to define the user identifiers.

var itemIdentifierColumn: String

The name of the column you selected at initialization to define the item identifiers.

var ratingColumn: String?

The name of the column you selected at initialization to define the ratings.

