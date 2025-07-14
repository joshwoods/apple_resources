

- ClockKit
- CLKComplicationServer
-  reloadTimeline(for:) Deprecated

Instance Method

# reloadTimeline(for:)

Invalidates your existing timeline data and triggers an update session to reload it.

watchOS 2.0–9.0Deprecated

``` source
func reloadTimeline(for complication: CLKComplication)
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Mentioned in 

Keeping your complications up to date

## Discussion

Call this method when your complication data is no longer accurate and needs to be completely replaced. ClockKit dumps any cached data and initiates a fresh update session to request new data from your complication data source. If your complication has already exceeded its allotted daily budget for execution time, calls to this method do nothing.

Call this method sparingly. If your existing complication data is still valid, consider calling the extendTimeline(for:) method instead.

## See Also

### Updating Your Timeline Data

func extendTimeline(for: CLKComplication)

Asks the system to extend the data in your complication’s timeline.

Deprecated

