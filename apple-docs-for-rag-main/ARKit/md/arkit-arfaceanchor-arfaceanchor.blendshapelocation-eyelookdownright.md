

- ARKit
- ARFaceAnchor
- ARFaceAnchor.BlendShapeLocation
-  eyeLookDownRight 

Type Property

# eyeLookDownRight

The coefficient describing movement of the right eyelids consistent with a downward gaze.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
static let eyeLookDownRight: ARFaceAnchor.BlendShapeLocation
```

## Discussion

The figure below shows a face geometry (see ARSCNFaceGeometry) in two states, demonstrating values of `0.0` and `1.0` for this coefficient. In both states, the values for all other ARFaceAnchor.BlendShapeLocation coefficients are set to `0.0`.

## See Also

### Right Eye

static let eyeBlinkRight: ARFaceAnchor.BlendShapeLocation

The coefficient describing closure of the eyelids over the right eye.

static let eyeLookInRight: ARFaceAnchor.BlendShapeLocation

The coefficient describing movement of the right eyelids consistent with a leftward gaze.

static let eyeLookOutRight: ARFaceAnchor.BlendShapeLocation

The coefficient describing movement of the right eyelids consistent with a rightward gaze.

static let eyeLookUpRight: ARFaceAnchor.BlendShapeLocation

The coefficient describing movement of the right eyelids consistent with an upward gaze.

static let eyeSquintRight: ARFaceAnchor.BlendShapeLocation

The coefficient describing contraction of the face around the right eye.

static let eyeWideRight: ARFaceAnchor.BlendShapeLocation

The coefficient describing a widening of the eyelids around the right eye.

