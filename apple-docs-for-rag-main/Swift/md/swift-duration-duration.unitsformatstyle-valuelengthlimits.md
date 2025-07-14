

- Swift
- Duration
- Duration.UnitsFormatStyle
-  valueLengthLimits 

Instance Property

# valueLengthLimits

The padding or truncating behavior of the unit value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var valueLengthLimits: Range?
```

## Discussion

For example, set this to `2...` to force 2-digit padding on all units.

## See Also

### Working with units

var allowedUnits: Set&lt;Duration.UnitsFormatStyle.Unit>

The units that may be included in the output string.

struct Unit

A unit to use in formatting a duration.

var maximumUnitCount: Int?

The maximum number of time units to include in the output string.

