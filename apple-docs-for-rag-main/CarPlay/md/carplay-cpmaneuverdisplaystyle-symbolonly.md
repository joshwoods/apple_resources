

- CarPlay
- CPManeuverDisplayStyle
-  symbolOnly 

Type Property

# symbolOnly

Only the symbol appears for the maneuver.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
static var symbolOnly: CPManeuverDisplayStyle { get }
```

## Discussion

If your app provides lane guidance, include a second maneuver to the navigation session’s upcomingManeuvers array that provides the lane guidance information. The second maneuver should have:

- A symbolSet containing dark and light images that fill the full width of the guidance panel with a maximum image size of 120 pt x 18 pt.

- An empty array of instructionVariants.

The map template should include a mapDelegate object that conforms to CPMapTemplateDelegate and implements the mapTemplate(_:displayStyleFor:) method, which returns the symbolOnly display style for the maneuver.

## See Also

### Display Styles

static var leadingSymbol: CPManeuverDisplayStyle

The symbol appears before the instructions for the maneuver.

static var trailingSymbol: CPManeuverDisplayStyle

The symbol appears after the instructions for the maneuver.

static var instructionOnly: CPManeuverDisplayStyle

Only the instructions appear for the maneuver.

