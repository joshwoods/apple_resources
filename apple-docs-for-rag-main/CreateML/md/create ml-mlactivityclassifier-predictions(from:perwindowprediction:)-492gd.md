

- Create ML
- MLActivityClassifier
-  predictions(from:perWindowPrediction:) 

Instance Method

# predictions(from:perWindowPrediction:)

Predict activities from new observations.

macOS 13.0+

``` source
func predictions(
    from data: DataFrame,
    perWindowPrediction: Bool? = false
) throws -> [String]
```

## Return Value

An array of predicted class names.

## Discussion

- Parameters

  - testingData: A data frame containing unlabeled sensor data samples. All samples are assumed to come from the same recording. Feature column names used in the table should be consistent with those used in training.

  - perWindowPrediction: A Boolean option to specify the prediction frequency. Default is false, and prediction is made per sample, instead of per window.

Throws

`MLCreateError.type` if `testingData` format is invalid.

## See Also

### Testing an activity classifier

func predictions(from: MLDataTable, perWindowPrediction: Bool?) throws -> [String]

Predict activities from new observations.

Deprecated

