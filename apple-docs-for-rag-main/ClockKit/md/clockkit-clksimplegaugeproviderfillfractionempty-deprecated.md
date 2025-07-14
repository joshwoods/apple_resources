

- ClockKit
-  CLKSimpleGaugeProviderFillFractionEmpty Deprecated

Global Variable

# CLKSimpleGaugeProviderFillFractionEmpty

A fill value indicating an empty gauge.

watchOS 5.0–9.0Deprecated

``` source
let CLKSimpleGaugeProviderFillFractionEmpty: Float
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Discussion

For CLKGaugeProviderStyle.ring style gauges, the CLKSimpleGaugeProviderFillFractionEmpty value hides the ring, while setting a `0.0` fill value still shows the ring.

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

enum CLKGaugeProviderStyle

Visual styles available for gauges.

Deprecated

