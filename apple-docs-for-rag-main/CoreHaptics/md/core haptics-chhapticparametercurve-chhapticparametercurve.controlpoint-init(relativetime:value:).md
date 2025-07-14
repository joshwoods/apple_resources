

- Core Haptics
- CHHapticParameterCurve
- CHHapticParameterCurve.ControlPoint
-  init(relativeTime:value:) 

Initializer

# init(relativeTime:value:)

Creates a control point from its time and value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
init(
    relativeTime time: TimeInterval,
    value: Float
)
```

## Parameters 

`time`  

The time at which the associated parameter reaches this value, relative to the parameter curve’s start time.

`value`  

The value of the parameter at this control point.

