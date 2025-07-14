

- Create ML Components
-  Classification 

Structure

# Classification

An item in a classification result.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct Classification where Label : Hashable
```

## Topics

### Creating the item

init(label: Label, probability: Float)

Creates a classification with label and probability.

### Getting the properties

var label: Label

The classification label.

var probability: Float

The classification probability. A value between 0 and 1.

### Operators

static func == (Classification&lt;Label>, Classification&lt;Label>) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Metrics

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

func meanAbsolutePercentageError&lt;T>([AnnotatedPrediction&lt;T, T>]) -> T

Computes the mean absolute percentage error between predicted and ground truth values.

func meanSquaredError&lt;T>([AnnotatedPrediction&lt;T, T>]) -> T

Computes the root mean squared error between predicted and ground truth values.

func meanSquaredError&lt;T>(some Collection, some Collection) -> T

Computes the mean squared error between predicted and ground truth values.

