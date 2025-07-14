

- Create ML
-  MLIdentifier Deprecated

Protocol

# MLIdentifier

A type the Create ML framework can use as a machine learning identifier.

macOS 10.15–14.0Deprecated

``` source
protocol MLIdentifier
```

## Overview

You can use any type that conforms to the MLIdentifier protocol, typically Int or String, to uniquely identify users and items in these MLRecommender methods:

- 

recommendations(fromUsers:maxCount:restrictingToItems:excluding:excludingObserved:)

- getSimilarItems(fromItems:maxCount:)

## Topics

### Getting an identifier

var identifierValue: MLDataValue

The value of the unique identifier wrapped in a data value.

**Required**

## See Also

### Testing a recommender

func recommendations&lt;T>(fromUsers: MLDataColumn&lt;T>, maxCount: Int, restrictingToItems: MLDataColumn&lt;T>?, excluding: MLDataTable?, excludingObserved: Bool) throws -> MLDataTable

Retrieves the highest scored items for the given column of users, based on item similarity and the rating column.

Deprecated

func recommendations(fromUsers: [any MLIdentifier], maxCount: Int, restrictingToItems: [any MLIdentifier]?, excluding: MLDataTable?, excludingObserved: Bool) throws -> MLDataTable

Retrieves the highest scored item for the given array of users, based on item similarity and the rating column.

Deprecated

func getSimilarItems&lt;T>(fromItems: MLDataColumn&lt;T>, maxCount: Int) throws -> MLDataTable

Returns the top ranked similar items based on the model’s similarity type.

Deprecated

func getSimilarItems(fromItems: [any MLIdentifier], maxCount: Int) throws -> MLDataTable

Returns the top ranked similar items based on the model’s similarity type.

Deprecated

