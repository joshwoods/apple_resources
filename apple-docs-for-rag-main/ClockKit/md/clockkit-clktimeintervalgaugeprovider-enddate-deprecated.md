

- ClockKit
- CLKTimeIntervalGaugeProvider
-  endDate Deprecated

Instance Property

# endDate

The ending time and date for the gauge’s time interval.

watchOS 5.0–9.0Deprecated

``` source
var endDate: Date { get }
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Discussion

The end date is equal to or later than the start date.

## See Also

### Getting Information about the Gauge

var startDate: Date

The starting time and date for the gauge’s time interval.

Deprecated

var startFillFraction: Float

The position of the leading edge of the time bar within the specified time interval.

Deprecated

var endFillFraction: Float

The position of the trailing edge of the time bar within the specified time interval.

Deprecated

