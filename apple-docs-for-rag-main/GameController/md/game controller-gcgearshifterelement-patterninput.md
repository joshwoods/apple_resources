

- Game Controller
- GCGearShifterElement
-  patternInput 

Instance Property

# patternInput

The input object for a pattern gear shift.

Mac Catalyst 16.0+macOS 13.0+

``` source
var patternInput: (any GCSwitchPositionInput)? { get }
```

## Discussion

If this property is `nil`, the gear shift isn’t a pattern gear shift. A pattern gear shift lays out the gears in a pattern that lets the user move to any gear. If the position property of this property is `0`, the gear shift is in neutral. If it’s `-1`, the gear shift is in reverse.

## See Also

### Accessing input values

var sequentialInput: (any GCRelativeInput)?

The input object for a sequential gear shift.

