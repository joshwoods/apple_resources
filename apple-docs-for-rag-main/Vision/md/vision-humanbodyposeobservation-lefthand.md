

- Vision
- HumanBodyPoseObservation
-  leftHand 

Instance Property

# leftHand

The observed left hand.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
let leftHand: HumanHandPoseObservation?
```

## See Also

### Inspecting an observation

enum RequestDescriptor

A type that describes the request and revision combination.

let rightHand: HumanHandPoseObservation?

The observed right hand.

struct HumanHandPoseObservation

An observation that provides the hand points the analysis recognizes.

var keypoints: MLMultiArray

A multi-array compatible with Core ML that contains normalized point coordinates and confidence scores.

