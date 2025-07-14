

- Game Controller
-  GCLinearInput 

Protocol

# GCLinearInput

The common properties of inputs that provide values in unit coordinates.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
protocol GCLinearInput : NSObjectProtocol
```

## Topics

### Getting the characteristics

var canWrap: Bool

A Boolean value that indicates whether the input value wraps when it reaches the range’s minimum or maximum value.

**Required**

var isAnalog: Bool

A Boolean value that indicates whether the input provides analog values.

**Required**

### Getting the value

var value: Float

The value in unit coordinates.

**Required**

var valueDidChangeHandler: ((any GCPhysicalInputElement, any GCLinearInput, Float) -> Void)?

The block that the profile calls when an element’s value changes.

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

