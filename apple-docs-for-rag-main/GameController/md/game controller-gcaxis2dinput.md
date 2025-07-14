

- Game Controller
-  GCAxis2DInput 

Protocol

# GCAxis2DInput

The common properties of inputs that provide a normalized point in a two-dimensional coordinate system with a fixed origin.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.3+tvOS 17.4+visionOS 1.1+

``` source
protocol GCAxis2DInput : NSObjectProtocol
```

## Overview

The normalized point with coordinates that range between `-1` and `1`. The origin `(0, 0)` represents the neutral state of the input.

## Topics

### Getting the characteristics

var canWrap: Bool

A Boolean value that indicates whether the value wraps when it reaches the range’s minimum or maximum value.

**Required**

var isAnalog: Bool

A Boolean value that indicates whether the input provides analog values.

**Required**

### Getting the value

var value: GCPoint2

The axis input represented as a normalized point in a two-dimensional coordinate system.

**Required**

struct GCPoint2

A structure that represents a normalized point in a two-dimensional coordinate system.

var valueDidChangeHandler: ((any GCPhysicalInputElement, any GCAxis2DInput, GCPoint2) -> Void)?

The block that the axis element calls when its value changes.

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

### Axes

var xAxis: any GCAxisInput

The input object that represents the x-axis on the directional pad.

**Required**

var yAxis: any GCAxisInput

The input object that represents the y-axis on the directional pad.

**Required**

var xyAxes: any GCAxis2DInput

The location of the directional pad represented as a point.

**Required**

