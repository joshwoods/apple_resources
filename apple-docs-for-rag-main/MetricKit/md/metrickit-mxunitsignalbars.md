

- MetricKit
-  MXUnitSignalBars 

Class

# MXUnitSignalBars

A unit of measure for the number of bars of cellular network connectivity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class MXUnitSignalBars
```

## Overview

Cellular connectivity measures the relative strength of the device’s signal reception in decibels, which usually falls in a range of 0 to -110.

`MXUnitSignalBars` defines the base unit as bars corresponding to the bars in the cellular connection status icon at the top of a device screen.

## Topics

### Measuring Connection Strength

class var bars: MXUnitSignalBars

The number of bars of connectivity to the cellular network.

## Relationships

### Inherits From

- Dimension

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Viewing cellular connectivity metrics

var histogrammedCellularConditionTime: MXHistogram&lt;MXUnitSignalBars>

An object representing the distribution of the different levels of connectivity to the cellular network.

