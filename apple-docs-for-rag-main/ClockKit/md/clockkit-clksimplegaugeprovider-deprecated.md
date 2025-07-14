

- ClockKit
-  CLKSimpleGaugeProvider Deprecated

Class

# CLKSimpleGaugeProvider

A gauge that shows a fractional value.

watchOS 5.0–9.0Deprecated

``` source
class CLKSimpleGaugeProvider
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Mentioned in 

Creating a timeline entry

## Overview

A simple gauge provider displays values that map to a `0.0` to `1.0` range. For example, you could use the gauge to show the percentage of a task that has been completed, or the current temperature within a specified temperature range.

Note

Tinted graphic complications display gauges using a solid color chosen by the user.

For time intervals, use the CLKTimeIntervalGaugeProvider.

## Topics

### Creating a Simple Gauge Provider

convenience init(style: CLKGaugeProviderStyle, gaugeColor: UIColor, fillFraction: Float)

Creates a solid-color gauge.

convenience init(style: CLKGaugeProviderStyle, gaugeColors: [UIColor]?, gaugeColorLocations: [NSNumber]?, fillFraction: Float)

Creates a multicolor gauge.

### Getting Information About the Gauge

var fillFraction: Float

The value displayed by the gauge.

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

class CLKTimeIntervalGaugeProvider

A gauge that tracks time intervals.

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

