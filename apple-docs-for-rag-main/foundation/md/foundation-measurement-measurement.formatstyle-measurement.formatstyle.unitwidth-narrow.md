

- Foundation
- Measurement
- Measurement.FormatStyle
- Measurement.FormatStyle.UnitWidth
-  narrow 

Type Property

# narrow

The shortest unit width.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var narrow: Measurement.FormatStyle.UnitWidth { get }
```

## Discussion

This width may condense the spacing between the value and the unit; for example, `37.20Cal` or `37,2L`.

## See Also

### Unit widths

static var wide: Measurement&lt;UnitType>.FormatStyle.UnitWidth

A unit width that shows the full unit name.

static var abbreviated: Measurement&lt;UnitType>.FormatStyle.UnitWidth

An abbreviated unit width.

