

- Swift
- Duration
- Duration.UnitsFormatStyle
-  Duration.UnitsFormatStyle.UnitWidth 

Structure

# Duration.UnitsFormatStyle.UnitWidth

The width of a unit to use in formatting a duration.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct UnitWidth
```

## Overview

Use the provided unit widths with the `width` parameter of the Duration.UnitsFormatStyle initializers to customize the display of units in a formatted string.

## Topics

### Duration unit widths

static var abbreviated: Duration.UnitsFormatStyle.UnitWidth

An abbreviated unit name.

static var condensedAbbreviated: Duration.UnitsFormatStyle.UnitWidth

An abbreviated unit name, with condensed space between the value and name.

static var narrow: Duration.UnitsFormatStyle.UnitWidth

The shortest possible unit name.

static var wide: Duration.UnitsFormatStyle.UnitWidth

The full unit name.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Working with unit widths

var unitWidth: Duration.UnitsFormatStyle.UnitWidth

The width of the unit and the spacing between the value and the unit.

