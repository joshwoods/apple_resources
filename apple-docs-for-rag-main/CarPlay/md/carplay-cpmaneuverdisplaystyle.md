

- CarPlay
-  CPManeuverDisplayStyle 

Structure

# CPManeuverDisplayStyle

A display style that determines the visual layout for a maneuver.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
struct CPManeuverDisplayStyle
```

## Topics

### Display Styles

static var leadingSymbol: CPManeuverDisplayStyle

The symbol appears before the instructions for the maneuver.

static var trailingSymbol: CPManeuverDisplayStyle

The symbol appears after the instructions for the maneuver.

static var instructionOnly: CPManeuverDisplayStyle

Only the instructions appear for the maneuver.

static var symbolOnly: CPManeuverDisplayStyle

Only the symbol appears for the maneuver.

### Initializers

init(rawValue: Int)

Initializes a maneuver display style using the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Setting the Display Style

func mapTemplate(CPMapTemplate, displayStyleFor: CPManeuver) -> CPManeuverDisplayStyle

Asks the delegate for the maneuver’s display style.

