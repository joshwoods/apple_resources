

- Create ML
- MLRecommender
-  getSimilarItems(fromItems:maxCount:) Deprecated

Instance Method

# getSimilarItems(fromItems:maxCount:)

Returns the top ranked similar items based on the model’s similarity type.

macOS 10.15–14.0Deprecated

``` source
func getSimilarItems(
    fromItems: [any MLIdentifier],
    maxCount: Int = 10
) throws -> MLDataTable
```

## Parameters 

`fromItems`  

An array of item identifiers.

`maxCount`  

The maximum number of similar items per item in the `fromItems` column. The default is `10`.

## See Also

### Testing a recommender

func recommendations&lt;T>(fromUsers: MLDataColumn&lt;T>, maxCount: Int, restrictingToItems: MLDataColumn&lt;T>?, excluding: MLDataTable?, excludingObserved: Bool) throws -> MLDataTable

Retrieves the highest scored items for the given column of users, based on item similarity and the rating column.

Deprecated

func recommendations(fromUsers: [any MLIdentifier], maxCount: Int, restrictingToItems: [any MLIdentifier]?, excluding: MLDataTable?, excludingObserved: Bool) throws -> MLDataTable

Retrieves the highest scored item for the given array of users, based on item similarity and the rating column.

Deprecated

protocol MLIdentifier

A type the Create ML framework can use as a machine learning identifier.

Deprecated

func getSimilarItems&lt;T>(fromItems: MLDataColumn&lt;T>, maxCount: Int) throws -> MLDataTable

Returns the top ranked similar items based on the model’s similarity type.

Deprecated

