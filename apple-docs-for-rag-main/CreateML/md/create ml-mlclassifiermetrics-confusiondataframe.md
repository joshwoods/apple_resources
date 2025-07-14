

- Create ML
- MLClassifierMetrics
-  confusionDataFrame 

Instance Property

# confusionDataFrame

A data frame comparing the actual and predicted labels for each class.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
var confusionDataFrame: DataFrame { get }
```

## Discussion

The confusion data frame describes how examples were mislabeled between categories. Each row contains the true label, the predicted label, and the number of instances of that combination. For example, the table below lists that “business” was labeled correctly with “business” 113 times, while “business” was confused with “entertainment” 2 times.

## See Also

### Understanding the model

var classificationError: Double

The fraction of incorrectly labeled examples.

var precisionRecall: MLDataTable

A data table listing the precision and recall percentages for each class.

var confusion: MLDataTable

A table comparing the actual and predicted labels for each classification category.

var precisionRecallDataFrame: DataFrame

A data frame listing the precision and recall percentages for each class.

