

- ClockKit
- CLKComplicationTimelineEntry
-  complicationTemplate Deprecated

Instance Property

# complicationTemplate

The template containing the data to display in your complication.

watchOS 2.0–9.0Deprecated

``` source
@NSCopying
var complicationTemplate: CLKComplicationTemplate { get set }
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Discussion

Specify a template that matches the style of complication for which you’re providing data. Different templates require different types of data. You must configure the template data before returning the timeline entry to ClockKit.

## See Also

### Setting the Entry Values

var date: Date

The time at which to display the entry.

Deprecated

var timelineAnimationGroup: String?

The animation group to which the entry belongs.

Deprecated

