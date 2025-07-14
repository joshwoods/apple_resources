

- Swift
- Duration
- Duration.UnitsFormatStyle
- Duration.UnitsFormatStyle.UnitWidth
-  abbreviated 

Type Property

# abbreviated

An abbreviated unit name.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static var abbreviated: Duration.UnitsFormatStyle.UnitWidth { get }
```

## Discussion

For example, `abbreviated` produces the unit label “3 hr” for a 3-hour duration in the `en_US` locale.

## See Also

### Duration unit widths

static var condensedAbbreviated: Duration.UnitsFormatStyle.UnitWidth

An abbreviated unit name, with condensed space between the value and name.

static var narrow: Duration.UnitsFormatStyle.UnitWidth

The shortest possible unit name.

static var wide: Duration.UnitsFormatStyle.UnitWidth

The full unit name.

