

- Create ML
- MLDecisionTreeClassifier
- MLDecisionTreeClassifier.ModelParameters
- MLDecisionTreeClassifier.ModelParameters.ValidationData
-  MLDecisionTreeClassifier.ModelParameters.ValidationData.dataFrame(\_:) 

Case

# MLDecisionTreeClassifier.ModelParameters.ValidationData.dataFrame(\_:)

Validation data provided in a DataFrame.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
case dataFrame(DataFrame)
```

## See Also

### Specifying validation data

case split(strategy: MLSplitStrategy)

Generate validation data by splitting the training dataset. This is the default.

case table(MLDataTable)

Set validation data from the MLDataTable provided.

case none

Do not set validation data.

