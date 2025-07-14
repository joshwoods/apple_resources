

- Game Controller
-  GCAxisInput 

Protocol

# GCAxisInput

The common properties of inputs that provide absolute values along an axis with a fixed origin.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
protocol GCAxisInput : NSObjectProtocol
```

## Topics

### Getting the characteristics

var canWrap: Bool

A Boolean value that indicates whether the value wraps when it reaches the range’s minimum or maximum value.

**Required**

var isAnalog: Bool

A Boolean value that indicates whether the input provides analog values.

**Required**

### Getting the value

var value: Float

The value along the axis, in unit coordinates.

**Required**

var valueDidChangeHandler: ((any GCPhysicalInputElement, any GCAxisInput, Float) -> Void)?

The block that the input object calls when the value changes.

**Required**

var lastValueTimestamp: TimeInterval

The time of the most recent value change.

**Required**

var lastValueLatency: TimeInterval

The time in seconds between the last value change and the current time.

**Required**

### Getting user actions

var sources: Set&lt;AnyHashable>

One or more physical actions the user performs to manipulate the input.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Gear shifter elements

class GCGearShifterElement

An element that represents either a pattern or a sequential gear shift.

protocol GCRelativeInput

The common properties of inputs that provide positions along an axis that are relative to the previous position.

