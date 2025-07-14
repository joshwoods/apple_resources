

- Game Controller
-  GCSwitchPositionInput 

Protocol

# GCSwitchPositionInput

The common properties of inputs that switch between two or more positions.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
protocol GCSwitchPositionInput : NSObjectProtocol
```

## Topics

### Getting the characteristics

var positionRange: NSRange

The range of possible values for the switch.

**Required**

var isSequential: Bool

A Boolean value that indicates whether the position change is sequential.

**Required**

var canWrap: Bool

A Boolean value that indicates whether the position value wraps when it reaches the range’s minimum or maximum value.

**Required**

### Getting the position

var position: Int

The position of the switch.

**Required**

var positionDidChangeHandler: ((any GCPhysicalInputElement, any GCSwitchPositionInput, Int) -> Void)?

The block that the profile calls when the value of the switch changes.

**Required**

var lastPositionTimestamp: TimeInterval

A timestamp for when the profile reports the last position.

**Required**

var lastPositionLatency: TimeInterval

The time in seconds between the current and previous positions.

**Required**

### Getting user actions

var sources: Set&lt;AnyHashable>

One or more physical actions the user performs to manipulate the input.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Steering and switch elements

class GCSteeringWheelElement

The element that represents the wheel of a racing wheel controller.

