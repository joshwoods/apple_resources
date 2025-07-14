

- Swift Charts
-  ChartBinRange 

Structure

# ChartBinRange

The range of data that a single bin of a chart represents.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct ChartBinRange where Bound : Comparable
```

## Overview

All bins except the last for a particular chart represent an open range, meaning that the range doesn’t include the upper bound. The last range of the last bin is closed, so that it does include the upper bound. The system keeps track of the open or closed state of a particular range.

## Topics

### Instance Properties

let lowerBound: Bound

let upperBound: Bound

## Relationships

### Conforms To

- RangeExpression

## See Also

### Data bins

struct NumberBins

A collection of bins for a chart that plots data against numbers.

struct DateBins

A collection of bins for a chart that plots data against dates.

