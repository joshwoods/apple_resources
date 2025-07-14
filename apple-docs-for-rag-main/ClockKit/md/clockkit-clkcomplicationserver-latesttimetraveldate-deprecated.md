

- ClockKit
- CLKComplicationServer
-  latestTimeTravelDate Deprecated

Instance Property

# latestTimeTravelDate

The latest date supported by Time Travel.

watchOS 2.0–7.0Deprecated

``` source
var latestTimeTravelDate: Date { get }
```

Deprecated

Time Travel is no longer supported.

## Discussion

When constructing your timeline, don’t create any entries after this date. Doing so is a waste of time because those entries won’t be displayed right away.

## See Also

### Getting the Time Travel Boundaries

var earliestTimeTravelDate: Date

The earliest Time Travel date for which you should provide data.

Deprecated

