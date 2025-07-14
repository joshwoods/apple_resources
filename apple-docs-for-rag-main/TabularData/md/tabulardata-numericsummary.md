

- TabularData
-  NumericSummary 

Structure

# NumericSummary

A summary of a numerical column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct NumericSummary where Element : BinaryFloatingPoint
```

## Topics

### Creating a Summary

init()

Creates an empty numeric summary with default values.

init(someCount: Int, noneCount: Int, mean: Element, standardDeviation: Element, min: Element, max: Element, median: Element, firstQuartile: Element, thirdQuartile: Element)

Creates an empty numeric summary.

### Comparing Summaries

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Inspecting a Summary

var debugDescription: String

A text representation of the summary’s statistics suitable for debugging.

var someCount: Int

The number of non-missing elements in the column.

var noneCount: Int

The number of missing elements in the column.

var totalCount: Int

The total number of elements in the column.

### Getting Statistical Values

var max: Element

The largest value, excluding missing elements.

var mean: Element

The arithmetic mean of a column’s values that excludes missing elements.

var median: Element

The midpoint value that’s above half of the non-missing elements’ values and below the other half’s values.

var min: Element

The smallest value, excluding missing elements.

var standardDeviation: Element

The standard deviation of a column’s values that excludes missing elements.

var firstQuartile: Element

The value that’s above 25% of the non-missing elements’ values.

var thirdQuartile: Element

The value that’s above 75% of the non-missing elements’ values.

### Operators

static func == (NumericSummary&lt;Element>, NumericSummary&lt;Element>) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- CustomDebugStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Statistical Summaries

struct CategoricalSummary

A categorical summary of a collection’s elements.

struct AnyCategoricalSummary

A type-erased categorical summary.

