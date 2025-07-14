

- Swift Charts
-  NumberBins 

Structure

# NumberBins

A collection of bins for a chart that plots data against numbers.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct NumberBins where Value : Comparable, Value : Numeric
```

## Topics

### Initializers

init(data: [Value], desiredCount: Int?, minimumStride: Value)

Automatically determine the bins from data.

init(data: [Value], desiredCount: Int?, minimumStride: Value)

Automatically determine the bins from data.

init(range: ClosedRange&lt;Value>, count: Int)

Creates the given number of bins for the range. Expects that the range length is a multiple of `count` to allow uniform integer bins.

init(range: ClosedRange&lt;Value>, count: Int)

Creates the given number of bins for the range.

init(range: ClosedRange&lt;Value>, desiredCount: Int, minimumStride: Value)

Automatically determine the bins from a range of data.

init(range: ClosedRange&lt;Value>, desiredCount: Int, minimumStride: Value)

Automatically determine the bins from a range of data.

init(size: Value, range: ClosedRange&lt;Value>)

Creates uniform bins covering the given range.

init(size: Value, range: ClosedRange&lt;Value>)

Creates uniform bins covering the given range.

init(thresholds: [Value])

Creates N-1 bins with the given N `thresholds`.

### Instance Properties

var thresholds: [Value]

Find the bin thresholds.

### Instance Methods

func index(for: Value) -> Int

Returns the bin index for the given value.

## Relationships

### Conforms To

- Collection
- Copyable
- Equatable
- Sequence

## See Also

### Data bins

struct DateBins

A collection of bins for a chart that plots data against dates.

struct ChartBinRange

The range of data that a single bin of a chart represents.

