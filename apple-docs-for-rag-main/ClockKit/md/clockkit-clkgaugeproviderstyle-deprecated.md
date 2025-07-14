

- ClockKit
-  CLKGaugeProviderStyle Deprecated

Enumeration

# CLKGaugeProviderStyle

Visual styles available for gauges.

watchOS 5.0–9.0Deprecated

``` source
enum CLKGaugeProviderStyle
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Topics

### Styles

case fill

A gauge that fills in as the value increases.

case ring

A gauge that indicates a value with a sliding ring.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Gauge providers

class CLKSimpleGaugeProvider

A gauge that shows a fractional value.

Deprecated

class CLKTimeIntervalGaugeProvider

A gauge that tracks time intervals.

Deprecated

class CLKGaugeProvider

An abstract superclass that provides all the common behaviors for the gauge providers.

Deprecated

let CLKSimpleGaugeProviderFillFractionEmpty: Float

A fill value indicating an empty gauge.

Deprecated

