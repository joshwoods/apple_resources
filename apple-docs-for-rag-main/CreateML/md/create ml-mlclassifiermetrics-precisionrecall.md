

- Create ML
- MLClassifierMetrics
-  precisionRecall 

Instance Property

# precisionRecall

A data table listing the precision and recall percentages for each class.

iOS 15.0–17.0DeprecatediPadOS 15.0–17.0DeprecatedMac Catalyst 15.0–17.0DeprecatedmacOS 10.14–14.0DeprecatedtvOS 16.0–17.0DeprecatedvisionOS 1.0+

``` source
var precisionRecall: MLDataTable { get }
```

## Mentioned in 

Improving Your Model’s Accuracy

## Discussion

Precision and recall are metrics calculated for each class. Together they describe the tradeoff between misapplying a label too liberally and missing examples of that label.

Precision describes how effective the model was at applying a label only when appropriate for a given category (few false positives).

Recall describes how effective the model was at finding all the relevant examples of a category (few false negatives).

The figure below shows how each example contributes to the precision and recall percentages for the category “Elephant”.

“Elephant” appears as the true or correct label only once, but it’s predicted twice. This second prediction is an error in precision. Precision and recall can give you a much better idea of how your model is making mistakes than classificationError.

To determine what other categories “Elephant” examples may have been labeled with, see the confusion property.

## See Also

### Understanding the model

var classificationError: Double

The fraction of incorrectly labeled examples.

var confusion: MLDataTable

A table comparing the actual and predicted labels for each classification category.

var confusionDataFrame: DataFrame

A data frame comparing the actual and predicted labels for each class.

var precisionRecallDataFrame: DataFrame

A data frame listing the precision and recall percentages for each class.

