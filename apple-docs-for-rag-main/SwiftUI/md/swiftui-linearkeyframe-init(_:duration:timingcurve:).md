

- SwiftUI
- LinearKeyframe
-  init(\_:duration:timingCurve:) 

Initializer

# init(\_:duration:timingCurve:)

Creates a new keyframe using the given value and timestamp.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init(
    _ to: Value,
    duration: TimeInterval,
    timingCurve: UnitCurve = .linear
)
```

## Parameters 

`to`  

The value of the keyframe.

`duration`  

The duration of the segment defined by this keyframe.

`timingCurve`  

A unit curve that controls the speed of interpolation.

