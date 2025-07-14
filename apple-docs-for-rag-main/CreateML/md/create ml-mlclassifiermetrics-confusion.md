

- Create ML
- MLClassifierMetrics
-  confusion 

Instance Property

# confusion

A table comparing the actual and predicted labels for each classification category.

iOS 15.0–17.0DeprecatediPadOS 15.0–17.0DeprecatedMac Catalyst 15.0–17.0DeprecatedmacOS 10.14–14.0DeprecatedtvOS 16.0–17.0DeprecatedvisionOS 1.0+

``` source
var confusion: MLDataTable { get }
```

## Mentioned in 

Improving Your Model’s Accuracy

## Discussion

The confusion data table describes how examples were mislabeled between categories. Each row contains the true label, the predicted label, and the count for each possible combination of categories. For example, the table below lists that “business” was labeled correctly with “business” 113 times, while “business” was confused with “entertainment” 2 times.

To gain insight into the performance of your model, you can use this data table to determine what categories your model is most confused about (making the most mistakes on) for a given data set. For example, the code listing below shows how to find the mistake that happens most frequently.

```
let confusion = model.validationMetrics.confusion

// Filter for rows which contain mistakes.
let errors = confusion[confusion["True Label"] != confusion["Predicted"]]
let mostCommonError = errors.rows.max { row1, row2 in
    row1["Count", Int.self]! 

Another useful view into this data is to compare the actual and predicated labels using a matrix. Printing the MLClassifierMetrics directly displays the matrix format.

```
print(model.validationMetrics)
// ...
// ******CONFUSION MATRIX******
// ----------------------------------
// True\Pred business entertainment politics sport tech
// business 113 2 3 0 9
// entertainment 1 183 3 2 3
// politics 6 8 116 0 3
// sport 0 6 1 135 3
// tech 2 7 3 0 129
// ...
```

In this example, the upper left hand count shows that 113 business examples were correctly labeled as “business”. The second column shows that “entertainment” was predicted for 2 “business” examples. The second row shows that 1 “entertainment” example was mislabeled as “business”.

## See Also

### Understanding the model

var classificationError: Double

The fraction of incorrectly labeled examples.

var precisionRecall: MLDataTable

A data table listing the precision and recall percentages for each class.

var confusionDataFrame: DataFrame

A data frame comparing the actual and predicted labels for each class.

var precisionRecallDataFrame: DataFrame

A data frame listing the precision and recall percentages for each class.

