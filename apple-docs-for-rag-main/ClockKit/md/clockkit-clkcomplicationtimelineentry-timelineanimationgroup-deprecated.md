

- ClockKit
- CLKComplicationTimelineEntry
-  timelineAnimationGroup Deprecated

Instance Property

# timelineAnimationGroup

The animation group to which the entry belongs.

watchOS 2.0–9.0Deprecated

``` source
var timelineAnimationGroup: String? { get set }
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Discussion

Use animation groups to created animated transitions between some, but not all, timeline entries. During Time Travel, ClockKit creates transition animations between entries with different group identifiers. ClockKit also creates transitions between entries whose identifiers are both `nil`. When the group identifiers are the same, ClockKit doesn’t create transition animations.

The group identifier is used only to determine whether transition animations should be created. The contents of the string may be anything that helps you identify the group to your app.

## See Also

### Setting the Entry Values

var date: Date

The time at which to display the entry.

Deprecated

var complicationTemplate: CLKComplicationTemplate

The template containing the data to display in your complication.

Deprecated

