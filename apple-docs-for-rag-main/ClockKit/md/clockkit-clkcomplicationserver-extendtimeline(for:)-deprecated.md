

- ClockKit
- CLKComplicationServer
-  extendTimeline(for:) Deprecated

Instance Method

# extendTimeline(for:)

Asks the system to extend the data in your complication’s timeline.

watchOS 2.0–9.0Deprecated

``` source
func extendTimeline(for complication: CLKComplication)
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Parameters 

`complication`  

The complication whose data you want to extend.

## Mentioned in 

Keeping your complications up to date

## Discussion

Call this method when your existing complication data is still valid and you’ve new data to add to the end of your timeline. ClockKit initiates an update session to request the additional data from your complication data source. If your complication has already exceeded its allotted daily budget for execution time, calls to this method do nothing.

## See Also

### Updating Your Timeline Data

func reloadTimeline(for: CLKComplication)

Invalidates your existing timeline data and triggers an update session to reload it.

Deprecated

