

- ClockKit
- CLKComplicationTimelineAnimationBehavior
-  CLKComplicationTimelineAnimationBehavior.always Deprecated

Case

# CLKComplicationTimelineAnimationBehavior.always

Always animate transitions. During Time Travel, ClockKit creates animations between all entries, regardless of the values of their group identifiers.

watchOS 2.0–9.0Deprecated

``` source
case always
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## See Also

### Constants

case never

No animations. This is the default behavior.

Deprecated

case grouped

Animations between groups. During Time Travel, ClockKit creates animations when transitioning between entries with different group identifiers. For entries with identical group identifiers, the new entry is displayed without animations.

Deprecated

