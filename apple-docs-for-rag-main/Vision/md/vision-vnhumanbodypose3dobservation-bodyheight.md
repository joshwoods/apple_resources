

- Vision
- VNHumanBodyPose3DObservation
-  bodyHeight 

Instance Property

# bodyHeight

The estimated human body height, in meters.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
var bodyHeight: Float { get }
```

## Mentioned in 

Identifying 3D human body poses in images

## Discussion

The framework returns an accurate height if heightEstimation is VNHumanBodyPose3DObservation.HeightEstimation.measured; otherwise, it returns a VNHumanBodyPose3DObservation.HeightEstimation.reference height.

## See Also

### Getting the Body Height

var heightEstimation: VNHumanBodyPose3DObservation.HeightEstimation

The technique the framework uses to estimate body height.

enum HeightEstimation

Constants that identify body height estimation techniques.

