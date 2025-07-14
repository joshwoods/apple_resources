

- Create ML
- MLRecommender
-  userIdentifierColumn 

Instance Property

# userIdentifierColumn

The name of the column you selected at initialization to define the user identifiers.

macOS 10.15+

``` source
var userIdentifierColumn: String
```

## Discussion

Changing the value of this property doesn’t retrain the model or affect its behavior.

## See Also

### Creating and training a recommender

init(trainingData: DataFrame, userColumn: String, itemColumn: String, ratingColumn: String?, parameters: MLRecommender.ModelParameters) throws

Creates an instance given a table and the names of the item and user columns contained therein.

init(trainingData: MLDataTable, userColumn: String, itemColumn: String, ratingColumn: String?, parameters: MLRecommender.ModelParameters) throws

Creates an instance given a table and the names of the item and user columns contained therein.

Deprecated

struct ModelParameters

Parameters that affect the process of training a recommender model.

let modelParameters: MLRecommender.ModelParameters

The configuration parameters that the recommender used for training during initialization.

var itemIdentifierColumn: String

The name of the column you selected at initialization to define the item identifiers.

var ratingColumn: String?

The name of the column you selected at initialization to define the ratings.

