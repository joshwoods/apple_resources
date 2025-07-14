

- Core Animation
- CAMediaTimingFunction
-  init(name:) 

Initializer

# init(name:)

Creates and returns a new instance of `CAMediaTimingFunction` configured with the predefined timing function specified by `name`.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
convenience init(name: CAMediaTimingFunctionName)
```

## Parameters 

`name`  

The timing function to use as specified in Predefined Timing Functions.

## Return Value

A new instance of `CAMediaTimingFunction` with the timing function specified by `name`.

## See Also

### Related Documentation

Core Animation Programming Guide

### Creating Timing Functions

init(controlPoints: Float, Float, Float, Float)

Returns an initialized timing function modeled as a cubic Bézier curve using the specified control points.

