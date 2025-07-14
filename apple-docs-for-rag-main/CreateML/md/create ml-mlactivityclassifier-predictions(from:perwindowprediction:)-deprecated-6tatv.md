

- Create ML
- MLActivityClassifier
-  predictions(from:perWindowPrediction:) Deprecated

Instance Method

# predictions(from:perWindowPrediction:)

Predict activities from new observations.

macOS 10.15–14.0Deprecated

``` source
func predictions(
    from data: MLDataTable,
    perWindowPrediction: Bool? = false
) throws -> [String]
```

## Parameters 

`data`  

A MLDataTable containing unlabeled sensor data samples. All samples are assumed to come from the same recording. Feature column names used in the table should be consistent with those used in training.

`perWindowPrediction`  

A Boolean option to specify the prediction frequency. Default is false, and prediction is made per sample, instead of per window.

## Return Value

An array of predicted class names.

## Discussion

Throws

`MLCreateError.type` if `testingData` format is invalid.

## See Also

### Testing an activity classifier

func predictions(from: DataFrame, perWindowPrediction: Bool?) throws -> [String]

Predict activities from new observations.

