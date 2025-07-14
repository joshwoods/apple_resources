

- Create ML Components
-  MultiLabelClassificationMetrics 

Structure

# MultiLabelClassificationMetrics

Multi-label classification metrics.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
struct MultiLabelClassificationMetrics where Label : Hashable
```

## Topics

### Creating the distribution

init(some Sequence&lt;(classification: ClassificationDistribution&lt;Label>, labels: Set&lt;Label>)>, strategy: MultiLabelClassificationMetrics&lt;Label>.ThresholdSelectionStrategy) throws

Creates multi-label classification metrics for classifications and ground truth labels.

init(some Sequence&lt;(classification: ClassificationDistribution&lt;Label>, labels: Set&lt;Label>)>, strategy: MultiLabelClassificationMetrics&lt;Label>.ThresholdSelectionStrategy, labels: Set&lt;Label>) throws

Creates multi-label classification metrics for classifications and ground truth labels.

init(classifications: some Sequence&lt;ClassificationDistribution&lt;Label>>, groundTruth: some Sequence&lt;Set&lt;Label>>, strategy: MultiLabelClassificationMetrics&lt;Label>.ThresholdSelectionStrategy) throws

Creates multi-label classification metrics for classifications and ground truth labels.

init(classifications: some Sequence&lt;ClassificationDistribution&lt;Label>>, groundTruth: some Sequence&lt;Set&lt;Label>>, strategy: MultiLabelClassificationMetrics&lt;Label>.ThresholdSelectionStrategy, labels: Set&lt;Label>) throws

Creates multi-label classification metrics for classifications and ground truth labels.

init(confidenceThresholds: [Label : Float])

Creates empty multi-label classification metrics.

enum ThresholdSelectionStrategy

A strategy for selecting a confidence threshold.

### Getting the properties

var confidenceThresholds: [Label : Float]

A dictionary of label and confidence thresholds.

var exampleCount: Int

The number of examples used to compute the metrics.

var labels: Set&lt;Label>

The classifier labels.

var meanAveragePrecision: Float

The mean average precision.

### Computing and scoring

func count(of: Label) -> Int

Returns the number of times a label appeared in the ground truth collection.

func f1Score(for: Label) -> Float

Computes the F1 score from predicted and ground truth values.

func falseNegativeCount(of: Label) -> Int

Returns the number of times a true label was not predicted.

func falsePositiveCount(of: Label) -> Int

Returns the number of times the predicted label did not match the true label.

func precisionScore(for: Label) -> Float

Computes the precision score for a class label.

func recallScore(for: Label) -> Float

Computes the recall score for a class label.

func trueNegativeCount(of: Label) -> Int

Returns the number of times a label was not in the predicted or ground truth collections.

func truePositiveCount(of: Label) -> Int

Returns the number of times the predicted label matched the true label.

### Updating the metrics

func add(some Sequence&lt;(classification: ClassificationDistribution&lt;Label>, labels: Set&lt;Label>)>)

Updates the metrics with more pairs of classifications and ground truth labels.

func add(classifications: some Sequence&lt;ClassificationDistribution&lt;Label>>, groundTruth: some Sequence&lt;Set&lt;Label>>)

Updates the metrics with more classifications and ground truth labels.

### Computing the precision

static func meanAveragePrecisionScore(some Sequence&lt;(classification: ClassificationDistribution&lt;Label>, labels: Set&lt;Label>)>) -> Float

Computes the mean average precision.

static func meanAveragePrecisionScore(some Sequence&lt;(classification: ClassificationDistribution&lt;Label>, labels: Set&lt;Label>)>, labels: Set&lt;Label>) -> Float

Computes the mean average precision.

static func meanAveragePrecisionScore(classifications: some Sequence&lt;ClassificationDistribution&lt;Label>>, groundTruth: some Sequence&lt;Set&lt;Label>>) -> Float

Computes the mean average precision.

static func meanAveragePrecisionScore(classifications: some Sequence&lt;ClassificationDistribution&lt;Label>>, groundTruth: some Sequence&lt;Set&lt;Label>>, labels: Set&lt;Label>) -> Float

Computes the mean average precision.

## Relationships

### Conforms To

- Sendable

## See Also

### Metrics

struct Classification

An item in a classification result.

struct ClassificationDistribution

A classification distribution that contains a probability for each classification label.

struct ClassificationMetrics

Classification metrics.

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

func meanAbsolutePercentageError&lt;T>([AnnotatedPrediction&lt;T, T>]) -> T

Computes the mean absolute percentage error between predicted and ground truth values.

func meanSquaredError&lt;T>([AnnotatedPrediction&lt;T, T>]) -> T

Computes the root mean squared error between predicted and ground truth values.

func meanSquaredError&lt;T>(some Collection, some Collection) -> T

Computes the mean squared error between predicted and ground truth values.

