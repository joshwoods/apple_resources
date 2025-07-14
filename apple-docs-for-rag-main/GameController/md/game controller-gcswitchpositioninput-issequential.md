

- Game Controller
- GCSwitchPositionInput
-  isSequential 

Instance Property

# isSequential

A Boolean value that indicates whether the position change is sequential.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var isSequential: Bool { get }
```

**Required**

## Discussion

A sequential gear shift requires the user to move through the gears in sequence.

## See Also

### Getting the characteristics

var positionRange: NSRange

The range of possible values for the switch.

**Required**

var canWrap: Bool

A Boolean value that indicates whether the position value wraps when it reaches the range’s minimum or maximum value.

**Required**

