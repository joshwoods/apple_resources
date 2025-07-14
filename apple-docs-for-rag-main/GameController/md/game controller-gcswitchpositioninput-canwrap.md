

- Game Controller
- GCSwitchPositionInput
-  canWrap 

Instance Property

# canWrap

A Boolean value that indicates whether the position value wraps when it reaches the range’s minimum or maximum value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var canWrap: Bool { get }
```

**Required**

## Discussion

For non-sequential switches, this property is always true.

## See Also

### Getting the characteristics

var positionRange: NSRange

The range of possible values for the switch.

**Required**

var isSequential: Bool

A Boolean value that indicates whether the position change is sequential.

**Required**

