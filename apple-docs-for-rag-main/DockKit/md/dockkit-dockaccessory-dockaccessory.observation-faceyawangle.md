

- DockKit
- DockAccessory
- DockAccessory.Observation
-  faceYawAngle 

Instance Property

# faceYawAngle

The angle of the face in radians.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
let faceYawAngle: Measurement?
```

## Discussion

A value of `0` indicates the face of the subject in the frame is looking directly at the camera. A negative value indicates the subject’s face is oriented to the left, while positive value indicates the face is oriented to the right.

## See Also

### Getting properties

let rect: CGRect

The coordinates of the subject in the frame.

let type: DockAccessory.Observation.ObservationType

The type of subject in the frame.

let identifier: Int

A unique identifier representing the subject in the frame.

