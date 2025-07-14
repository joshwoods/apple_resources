

- CarPlay
- CPMapTemplateDelegate
-  mapTemplate(\_:displayStyleFor:) 

Instance Method

# mapTemplate(\_:displayStyleFor:)

Asks the delegate for the maneuver’s display style.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
optional func mapTemplate(
    _ mapTemplate: CPMapTemplate,
    displayStyleFor maneuver: CPManeuver
) -> CPManeuverDisplayStyle
```

## Parameters 

`mapTemplate`  

The current map template.

`maneuver`  

The maneuver that the system applies the display style to.

## Return Value

A display style that determines the visual layout for the maneuver.

## Discussion

The display style only applies to the second maneuver that you provide in the navigation session’s upcomingManeuvers array.

## See Also

### Setting the Display Style

struct CPManeuverDisplayStyle

A display style that determines the visual layout for a maneuver.

