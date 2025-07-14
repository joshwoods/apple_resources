

- Vision
- VNClassificationObservation
-  hasMinimumPrecision(\_:forRecall:) 

Instance Method

# hasMinimumPrecision(\_:forRecall:)

Determines whether the observation for a specific recall has a minimum precision value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
func hasMinimumPrecision(
    _ minimumPrecision: Float,
    forRecall recall: Float
) -> Bool
```

## Parameters 

`minimumPrecision`  

The minimum percentage of classification results that are relevant.

`recall`  

The percentage of relevant results that the algorithm correctly classified.

## Return Value

A Boolean indicating whether or not this classification observation provides a minimum percentage of relevant results that meet the desired recall criterion.

## See Also

### Measuring Confidence and Precision

var hasPrecisionRecallCurve: Bool

A Boolean variable indicating whether the observation contains precision and recall curves.

func hasMinimumRecall(Float, forPrecision: Float) -> Bool

Determines whether the observation for a specific precision has a minimum recall value.

