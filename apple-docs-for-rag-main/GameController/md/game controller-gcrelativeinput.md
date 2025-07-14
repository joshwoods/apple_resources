

- Game Controller
-  GCRelativeInput 

Protocol

# GCRelativeInput

The common properties of inputs that provide positions along an axis that are relative to the previous position.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
protocol GCRelativeInput : NSObjectProtocol
```

## Topics

### Getting the characteristics

var isAnalog: Bool

A Boolean value that indicates whether the input provides analog values.

**Required**

### Getting the delta value and timestamp

var delta: Float

The most recent amount of change in values that the profile records.

**Required**

var deltaDidChangeHandler: ((any GCPhysicalInputElement, any GCRelativeInput, Float) -> Void)?

The block that the profile calls when the element’s input changes.

**Required**

var lastDeltaTimestamp: TimeInterval

A timestamp for when the profile reports the delta value.

**Required**

var lastDeltaLatency: TimeInterval

The time in seconds between the current and the previous delta values.

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

protocol GCAxisInput

The common properties of inputs that provide absolute values along an axis with a fixed origin.

class GCGearShifterElement

An element that represents either a pattern or a sequential gear shift.

