

- Vision
- HumanBodyPoseObservation
-  keypoints 

Instance Property

# keypoints

A multi-array compatible with Core ML that contains normalized point coordinates and confidence scores.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var keypoints: MLMultiArray { get throws }
```

## See Also

### Inspecting an observation

enum RequestDescriptor

A type that describes the request and revision combination.

let leftHand: HumanHandPoseObservation?

The observed left hand.

let rightHand: HumanHandPoseObservation?

The observed right hand.

struct HumanHandPoseObservation

An observation that provides the hand points the analysis recognizes.

