

- Create ML Components
-  meanAbsolutePercentageError(\_:) 

Function

# meanAbsolutePercentageError(\_:)

Computes the mean absolute percentage error between predicted and ground truth values.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func meanAbsolutePercentageError(_ annotatedPredictions: [AnnotatedPrediction]) -> T where T : FloatingPoint
```

## Parameters 

`annotatedPredictions`  

An `AnnotatedPrediction` object.

## Return Value

The mean absolute percentage error as a decimal value.

## Discussion

If an empty `AnnotatedPrediction` is supplied, the result will be NaN.

## See Also

### Metrics

struct Classification

An item in a classification result.

struct ClassificationDistribution

A classification distribution that contains a probability for each classification label.

struct ClassificationMetrics

Classification metrics.

struct MultiLabelClassificationMetrics

Multi-label classification metrics.

func rootMeanSquaredError&lt;T>([AnnotatedPrediction&lt;T, T>]) -> T

Computes the root mean squared error between predicted and ground truth values.

func rootMeanSquaredError&lt;T>(some Collection, some Collection) -> T

Computes the root mean squared error between predicted and ground truth values.

func maximumAbsoluteError&lt;T>([AnnotatedPrediction&lt;T, T>]) -> T

Computes the maximum absolute error between predicted and ground truth values.

func maximumAbsoluteError&lt;T>(some Collection, some Collection) -> T

Computes the maximum absolute error between predicted and ground truth values.

func meanAbsoluteError&lt;T>([AnnotatedPrediction&lt;T, T>]) -> T

Computes the mean absolute error between predicted and ground truth values.

func meanAbsoluteError&lt;T>(some Collection, some Collection) -> T

Computes the mean absolute error between predicted and ground truth values.

func meanSquaredError&lt;T>([AnnotatedPrediction&lt;T, T>]) -> T

Computes the root mean squared error between predicted and ground truth values.

func meanSquaredError&lt;T>(some Collection, some Collection) -> T

Computes the mean squared error between predicted and ground truth values.

