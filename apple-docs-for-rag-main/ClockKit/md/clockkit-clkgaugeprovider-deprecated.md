

- ClockKit
-  CLKGaugeProvider Deprecated

Class

# CLKGaugeProvider

An abstract superclass that provides all the common behaviors for the gauge providers.

watchOS 5.0–9.0Deprecated

``` source
class CLKGaugeProvider
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

Don’t create instances of this class yourself. Instead, create instances of the concrete subclasses based on the type of gauge you’re trying to create.

## Topics

### Setting the Gauge’s Appearance

var gaugeColors: [UIColor]?

The colors of the gauge.

var gaugeColorLocations: [NSNumber]?

The location of each color in a multicolor gauge’s gradient.

var style: CLKGaugeProviderStyle

The style that defines the gauge’s appearance.

### Adding Accessibility

var accessibilityLabel: String?

A localized string that describes the gague.

## Relationships

### Inherits From

- NSObject

### Inherited By

- CLKSimpleGaugeProvider
- CLKTimeIntervalGaugeProvider

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

class CLKTimeIntervalGaugeProvider

A gauge that tracks time intervals.

Deprecated

let CLKSimpleGaugeProviderFillFractionEmpty: Float

A fill value indicating an empty gauge.

Deprecated

enum CLKGaugeProviderStyle

Visual styles available for gauges.

Deprecated

