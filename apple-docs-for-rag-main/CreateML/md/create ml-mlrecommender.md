

- Create ML
-  MLRecommender 

Structure

# MLRecommender

A model you train to make recommendations based on item similarity, grouping, and, optionally, item ratings.

macOS 10.15+

``` source
struct MLRecommender
```

## Overview

Use an MLRecommender to train a machine learning model that you include in your app to make recommendations for the user, while keeping their data on-device.

You create a recommender model by training it with tabular data that includes columns for the recommendation items and the groups the items belong to. You also have the option to include an item rating column, which gives higher-rated items more weight than those with lesser or negative ratings. The recommender uses the training information to find similarity patterns by looking at items that occur in groups or have similar ratings within groups.

After you train a recommender, you save it as a Core ML model file with the `.mlmodel` extension. Import this model file into your Xcode project by dragging it into the Project navigator. At runtime, use the recommender to make item suggestions to the user based on the patterns in training data and the user’s item history. For example, a hiking app can recommend trails based on the trails a user has previously hiked and their ratings of those trails.

## Topics

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

var userIdentifierColumn: String

The name of the column you selected at initialization to define the user identifiers.

var itemIdentifierColumn: String

The name of the column you selected at initialization to define the item identifiers.

var ratingColumn: String?

The name of the column you selected at initialization to define the ratings.

### Evaluating a recommender

func evaluation(on: MLDataTable, userColumn: String, itemColumn: String, ratingColumn: String?, cutoffs: [Int], excludingObserved: Bool) -> MLRecommenderMetrics

Computes the metrics for the given testing data.

Deprecated

func evaluation(on: DataFrame, userColumn: String, itemColumn: String, ratingColumn: String?, cutoffs: [Int], excludingObserved: Bool) -> MLRecommenderMetrics

Computes the metrics for the given testing data.

struct MLRecommenderMetrics

Metrics you use to evaluate a recommender’s performance.

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

func getSimilarItems(fromItems: [any MLIdentifier], maxCount: Int) throws -> MLDataTable

Returns the top ranked similar items based on the model’s similarity type.

Deprecated

### Saving a recommender

func write(to: URL, metadata: MLModelMetadata?) throws

Exports the recommender as a Core ML model file at the given URL.

func write(toFile: String, metadata: MLModelMetadata?) throws

Exports the recommender as a Core ML model file at the given file path.

### Describing a recommender

var model: MLModel

The Core ML model.

### Enumerations

enum ModelAlgorithmType

The algorithms a recommender can use to make recommendations.

enum SimilarityType

The metric by which the recommender computes item similarity.

## See Also

### Tabular Models

Creating a Model from Tabular Data

Train a machine learning model by using Core ML to import and manage tabular data.

enum MLClassifier

A model you train to classify data into discrete categories.

enum MLRegressor

A model you train to estimate continuous values.

