

- ClockKit
- CLKComplicationTimelineEntry
-  date Deprecated

Instance Property

# date

The time at which to display the entry.

watchOS 2.0–9.0Deprecated

``` source
var date: Date { get set }
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Mentioned in 

Loading future timeline events

## Discussion

The date you specify represents the day and time at which to begin displaying the associated complication data. Set this value appropriately based on the data you want to display. For example, weather forecast data would use the time at which the forecast was valid, but information about an upcoming meeting would use an earlier date to give the user advance notice.

## See Also

### Setting the Entry Values

var complicationTemplate: CLKComplicationTemplate

The template containing the data to display in your complication.

Deprecated

var timelineAnimationGroup: String?

The animation group to which the entry belongs.

Deprecated

