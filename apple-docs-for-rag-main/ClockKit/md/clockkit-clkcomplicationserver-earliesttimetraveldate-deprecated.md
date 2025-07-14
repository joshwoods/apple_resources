

- ClockKit
- CLKComplicationServer
-  earliestTimeTravelDate Deprecated

Instance Property

# earliestTimeTravelDate

The earliest Time Travel date for which you should provide data.

watchOS 2.0–7.0Deprecated

``` source
var earliestTimeTravelDate: Date { get }
```

Deprecated

Time Travel is no longer supported.

## Discussion

When constructing your timeline, don’t create any entries before this date. Doing so is a waste of time because those entries will never be displayed.

## See Also

### Getting the Time Travel Boundaries

var latestTimeTravelDate: Date

The latest date supported by Time Travel.

Deprecated

