

- Game Controller
- GCSwitchPositionInput
-  positionDidChangeHandler 

Instance Property

# positionDidChangeHandler

The block that the profile calls when the value of the switch changes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var positionDidChangeHandler: ((any GCPhysicalInputElement, any GCSwitchPositionInput, Int) -> Void)? { get set }
```

**Required**

## Discussion

The block’s parameters are:

`element`  
The element whose position changes.

`input`  
The input object that represents the position.

`position`  
The new position of the element.

## See Also

### Getting the position

var position: Int

The position of the switch.

**Required**

var lastPositionTimestamp: TimeInterval

A timestamp for when the profile reports the last position.

**Required**

var lastPositionLatency: TimeInterval

The time in seconds between the current and previous positions.

**Required**

