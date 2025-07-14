

- Create ML
- MLRecommender
-  modelParameters 

Instance Property

# modelParameters

The configuration parameters that the recommender used for training during initialization.

macOS 10.15+

``` source
let modelParameters: MLRecommender.ModelParameters
```

## See Also

### Creating and training a recommender

init(trainingData: DataFrame, userColumn: String, itemColumn: String, ratingColumn: String?, parameters: MLRecommender.ModelParameters) throws

Creates an instance given a table and the names of the item and user columns contained therein.

init(trainingData: MLDataTable, userColumn: String, itemColumn: String, ratingColumn: String?, parameters: MLRecommender.ModelParameters) throws

Creates an instance given a table and the names of the item and user columns contained therein.

Deprecated

struct ModelParameters

Parameters that affect the process of training a recommender model.

var userIdentifierColumn: String

The name of the column you selected at initialization to define the user identifiers.

var itemIdentifierColumn: String

The name of the column you selected at initialization to define the item identifiers.

var ratingColumn: String?

The name of the column you selected at initialization to define the ratings.

