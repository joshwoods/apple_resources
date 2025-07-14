

- Create ML Components
-  ClassificationDistribution 

Structure

# ClassificationDistribution

A classification distribution that contains a probability for each classification label.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct ClassificationDistribution where Label : Hashable
```

## Topics

### Creating the distribution

init&lt;C>(C)

Creates a classification distribution.

### Getting the properties

var endIndex: Int

The index of the final element in the classification distribution.

var labelsSortedByProbability: [Label]

The labels sorted by decreasing probability.

var mostLikelyLabel: Label?

The label with the highest probability.

var startIndex: Int

The index of the initial element in the classification distribution.

### Getting the index

func index(after: Int) -> Int

Returns the index immediately after an element index.

func index(before: Int) -> Int

Returns the index immediately before an element index.

### Labeling and mapping

func topLabels(Int) -> [Label]

Computes the most likely labels in the classification set.

func map&lt;T>((Classification&lt;Label>) throws -> Classification&lt;T>) rethrows -> ClassificationDistribution&lt;T>

Creates a new classification distribution by applying a transformation to every element.

### Accessing by subscript

subscript(Range&lt;Int>) -> Slice&lt;ClassificationDistribution&lt;Label>>

Accesses a contiguous range of elements.

subscript(Int) -> Classification&lt;Label>

Accesses a classification at an index.

subscript(Label) -> Float?

Accesses a probability with label.

### Type Aliases

typealias Element

A type representing the sequence’s elements.

typealias Index

A type that represents a position in the collection.

typealias Indices

A type that represents the indices that are valid for subscripting the collection, in ascending order.

typealias Iterator

A type that provides the collection’s iteration interface and encapsulates its iteration state.

typealias SubSequence

A collection representing a contiguous subrange of this collection’s elements. The subsequence shares indices with the original collection.

### Default Implementations

Collection Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

Hashable Implementations

Sequence Implementations

## Relationships

### Conforms To

- Collection
- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable
- Sequence

## See Also

### Metrics

struct Classification

An item in a classification result.

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

