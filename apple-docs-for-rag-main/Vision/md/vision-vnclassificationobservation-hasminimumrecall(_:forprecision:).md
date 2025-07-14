

- Vision
- VNClassificationObservation
-  hasMinimumRecall(\_:forPrecision:) 

Instance Method

# hasMinimumRecall(\_:forPrecision:)

Determines whether the observation for a specific precision has a minimum recall value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
func hasMinimumRecall(
    _ minimumRecall: Float,
    forPrecision precision: Float
) -> Bool
```

## Parameters 

`minimumRecall`  

The minimum percentage of relevant results that the algorithm correctly classified.

`precision`  

The percentage of classification results that are relevant.

## Return Value

A Boolean indicating whether or not this classification observation provides a minimum percentage of relevant results that meet the desired precision criterion.

## See Also

### Measuring Confidence and Precision

var hasPrecisionRecallCurve: Bool

A Boolean variable indicating whether the observation contains precision and recall curves.

func hasMinimumPrecision(Float, forRecall: Float) -> Bool

Determines whether the observation for a specific recall has a minimum precision value.

