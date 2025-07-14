

- Create ML
- MLClassifierMetrics
-  init(classificationError:confusion:precisionRecall:) 

Initializer

# init(classificationError:confusion:precisionRecall:)

Creates empty classifier metrics.

iOS 15.0–17.0DeprecatediPadOS 15.0–17.0DeprecatedMac Catalyst 15.0–17.0DeprecatedmacOS 10.14–14.0DeprecatedtvOS 16.0–17.0DeprecatedvisionOS 1.0+

``` source
init(
    classificationError: Double,
    confusion: MLDataTable,
    precisionRecall: MLDataTable
)
```

## Parameters 

`classificationError`  

The fraction of incorrectly labeled examples.

`confusion`  

A confusion matrix describing the classifications for each category.

`precisionRecall`  

A two-dimensional table describing the precision and recall for each category.

## Discussion

You typically don’t initialize metrics directly. Instead you get metrics about your model after training. For example, when you train an MLClassifier, you can look at its trainingMetrics and validationMetrics properties. Additionally, you can check the performance on a test set with the evaluation(on:) method.

Warning

This initializer should not be used, it creates an empty instance.

