

- ClockKit
-  CLKTimeIntervalGaugeProvider Deprecated

Class

# CLKTimeIntervalGaugeProvider

A gauge that tracks time intervals.

watchOS 5.0–9.0Deprecated

``` source
class CLKTimeIntervalGaugeProvider
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Mentioned in 

Creating a timeline entry

## Overview

Use this gauge provider to visually show the amount of time that has elapsed within the specified time interval.

Note

Tinted graphic complications display gauges using a solid color chosen by the user.

## Topics

### Creating a Time Interval Gauge

convenience init(style: CLKGaugeProviderStyle, gaugeColors: [UIColor]?, gaugeColorLocations: [NSNumber]?, start: Date, end: Date)

Creates a time interval gauge that fills as time passes.

convenience init(style: CLKGaugeProviderStyle, gaugeColors: [UIColor]?, gaugeColorLocations: [NSNumber]?, start: Date, startFillFraction: Float, end: Date, endFillFraction: Float)

Creates a time interval gauge, letting you specify whether the gauge fills or empties as time passes.

### Getting Information about the Gauge

var startDate: Date

The starting time and date for the gauge’s time interval.

var endDate: Date

The ending time and date for the gauge’s time interval.

var startFillFraction: Float

The position of the leading edge of the time bar within the specified time interval.

var endFillFraction: Float

The position of the trailing edge of the time bar within the specified time interval.

## Relationships

### Inherits From

- CLKGaugeProvider

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Gauge providers

class CLKSimpleGaugeProvider

A gauge that shows a fractional value.

Deprecated

class CLKGaugeProvider

An abstract superclass that provides all the common behaviors for the gauge providers.

Deprecated

let CLKSimpleGaugeProviderFillFractionEmpty: Float

A fill value indicating an empty gauge.

Deprecated

enum CLKGaugeProviderStyle

Visual styles available for gauges.

Deprecated

