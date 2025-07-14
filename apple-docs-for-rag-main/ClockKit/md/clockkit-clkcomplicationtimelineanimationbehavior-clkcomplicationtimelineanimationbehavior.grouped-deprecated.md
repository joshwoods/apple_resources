

- ClockKit
- CLKComplicationTimelineAnimationBehavior
-  CLKComplicationTimelineAnimationBehavior.grouped Deprecated

Case

# CLKComplicationTimelineAnimationBehavior.grouped

Animations between groups. During Time Travel, ClockKit creates animations when transitioning between entries with different group identifiers. For entries with identical group identifiers, the new entry is displayed without animations.

watchOS 2.0–9.0Deprecated

``` source
case grouped
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## See Also

### Constants

case never

No animations. This is the default behavior.

Deprecated

case always

Always animate transitions. During Time Travel, ClockKit creates animations between all entries, regardless of the values of their group identifiers.

Deprecated

