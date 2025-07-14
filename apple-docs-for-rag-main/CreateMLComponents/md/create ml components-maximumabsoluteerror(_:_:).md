

- Create ML Components
-  maximumAbsoluteError(\_:\_:) 

Function

# maximumAbsoluteError(\_:\_:)

Computes the maximum absolute error between predicted and ground truth values.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
@backDeployed(before: macOS 14.0, iOS 17.0, tvOS 17.0)
func maximumAbsoluteError(
    _ predicted: some Collection,
    _ groundTruth: some Collection
) -> T where T : FloatingPoint
```

## Parameters 

`predicted`  

The predicted values.

`groundTruth`  

The ground truth values. The collection must have same number of elements as the predicted values.

## Return Value

The maximum absolute error.

## Discussion

Empty collections of predicted and ground truth values will return a value of NaN.

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

func meanAbsoluteError&lt;T>([AnnotatedPrediction&lt;T, T>]) -> T

Computes the mean absolute error between predicted and ground truth values.

func meanAbsoluteError&lt;T>(some Collection, some Collection) -> T

Computes the mean absolute error between predicted and ground truth values.

func meanAbsolutePercentageError&lt;T>([AnnotatedPrediction&lt;T, T>]) -> T

Computes the mean absolute percentage error between predicted and ground truth values.

func meanSquaredError&lt;T>([AnnotatedPrediction&lt;T, T>]) -> T

Computes the root mean squared error between predicted and ground truth values.

func meanSquaredError&lt;T>(some Collection, some Collection) -> T

Computes the mean squared error between predicted and ground truth values.

