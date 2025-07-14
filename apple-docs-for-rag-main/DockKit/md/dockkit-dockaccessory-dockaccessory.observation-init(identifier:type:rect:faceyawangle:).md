

- DockKit
- DockAccessory
- DockAccessory.Observation
-  init(identifier:type:rect:faceYawAngle:) 

Initializer

# init(identifier:type:rect:faceYawAngle:)

Creates a new observation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
init(
    identifier: Int,
    type: DockAccessory.Observation.ObservationType,
    rect: CGRect,
    faceYawAngle: Measurement? = nil
)
```

## Parameters 

`identifier`  

A unique identifier representing the subject in the frame.

`type`  

The type of subject in the frame.

`rect`  

The coordinates of the subject in the frame.

`faceYawAngle`  

The angle of the subject’s face in radians.

