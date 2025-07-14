

- Create ML
- MLClassifierMetrics
-  classificationError 

Instance Property

# classificationError

The fraction of incorrectly labeled examples.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
var classificationError: Double { get }
```

## Mentioned in 

Creating a Text Classifier Model

Improving Your Model’s Accuracy

Creating a text classifier model

## Discussion

The classification error describes how many examples were incorrectly labeled divided by the total number of examples. Accuracy as a percentage may be more intuitive. You can calculate it as follows:

```
let accuracy = (1 - metrics.classificationError) * 100
```

Important

This is a useful metric only when the data is well-balanced between categories. For example, suppose you build a classifier to detect a rare disease with very few examples of sick patients compared to the number of healthy patients. Predicting that a new patient will always be healthy would be highly accurate (low classification error), but a poor disease detector. The precisionRecall and confusion properties provide more detail in these cases.

## See Also

### Understanding the model

var precisionRecall: MLDataTable

A data table listing the precision and recall percentages for each class.

var confusion: MLDataTable

A table comparing the actual and predicted labels for each classification category.

var confusionDataFrame: DataFrame

A data frame comparing the actual and predicted labels for each class.

var precisionRecallDataFrame: DataFrame

A data frame listing the precision and recall percentages for each class.

