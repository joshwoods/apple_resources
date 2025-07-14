

- Swift Charts
-  DateBins 

Structure

# DateBins

A collection of bins for a chart that plots data against dates.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct DateBins
```

## Topics

### Initializers

init(data: [Date], desiredCount: Int?, calendar: Calendar)

Automatically determine the bins from data.

init(range: ClosedRange&lt;Date>, desiredCount: Int, calendar: Calendar)

Automatically determine the bins from a range of data.

init(thresholds: [Date])

Creates N-1 bins with the given N `thresholds`.

init(timeInterval: TimeInterval, range: ClosedRange&lt;Date>)

Creates uniform bins covering the given range. The first bin starts at the lower bound of the range.

init(unit: Calendar.Component, by: Int, range: ClosedRange&lt;Date>, calendar: Calendar)

Creates uniform bins covering the given range.

### Instance Properties

var thresholds: [Date]

Find the bin thresholds.

### Instance Methods

func index(for: Date) -> Int

Returns the bin index for the given value.

## Relationships

### Conforms To

- Collection
- Copyable
- Equatable
- Sequence

## See Also

### Data bins

struct NumberBins

A collection of bins for a chart that plots data against numbers.

struct ChartBinRange

The range of data that a single bin of a chart represents.

