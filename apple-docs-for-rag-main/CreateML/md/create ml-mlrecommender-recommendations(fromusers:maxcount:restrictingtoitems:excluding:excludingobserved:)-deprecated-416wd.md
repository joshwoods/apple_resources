

- Create ML
- MLRecommender
-  recommendations(fromUsers:maxCount:restrictingToItems:excluding:excludingObserved:) Deprecated

Instance Method

# recommendations(fromUsers:maxCount:restrictingToItems:excluding:excludingObserved:)

Retrieves the highest scored items for the given column of users, based on item similarity and the rating column.

macOS 10.15–14.0Deprecated

``` source
func recommendations(
    fromUsers: MLDataColumn,
    maxCount: Int = 10,
    restrictingToItems: MLDataColumn? = nil,
    excluding userItemObservations: MLDataTable? = nil,
    excludingObserved: Bool = true
) throws -> MLDataTable where T : MLDataValueConvertible, T : MLIdentifier
```

## Parameters 

`fromUsers`  

A column of user identifiers.

`maxCount`  

The maximum number of recommendations per user. The default is `10`.

`restrictingToItems`  

An array of item identifiers that defines the only values the recommender can use this set of recommendations. By default, the parameter is `nil`, meaning there are no restrictions.

`userItemObservations`  

A data table of user-item observations to exclude from recommendations.

The default is `nil`, meaning no observations are excluded.

The column names for the user identifiers and item identifiers must be the same as those provided in the training data.

`excludingObserved`  

Set this value to `true` to omit training data from the recommendations, or `false` to include them.

The default is `true`.

## Return Value

An MLDataTable containing columns with user identifiers, item identifiers, scores and ranks (numbered between `1` and the `maxCount`).

## See Also

### Testing a recommender

func recommendations(fromUsers: [any MLIdentifier], maxCount: Int, restrictingToItems: [any MLIdentifier]?, excluding: MLDataTable?, excludingObserved: Bool) throws -> MLDataTable

Retrieves the highest scored item for the given array of users, based on item similarity and the rating column.

Deprecated

protocol MLIdentifier

A type the Create ML framework can use as a machine learning identifier.

Deprecated

func getSimilarItems&lt;T>(fromItems: MLDataColumn&lt;T>, maxCount: Int) throws -> MLDataTable

Returns the top ranked similar items based on the model’s similarity type.

Deprecated

func getSimilarItems(fromItems: [any MLIdentifier], maxCount: Int) throws -> MLDataTable

Returns the top ranked similar items based on the model’s similarity type.

Deprecated

