

- Game Controller
- GCGearShifterElement
-  sequentialInput 

Instance Property

# sequentialInput

The input object for a sequential gear shift.

Mac Catalyst 16.0+macOS 13.0+

``` source
var sequentialInput: (any GCRelativeInput)? { get }
```

## Discussion

If this property is `nil`, this gear shift isn’t a sequential gear shift. A sequential gear shift requires the user to move through the gears in sequence.

## See Also

### Accessing input values

var patternInput: (any GCSwitchPositionInput)?

The input object for a pattern gear shift.

