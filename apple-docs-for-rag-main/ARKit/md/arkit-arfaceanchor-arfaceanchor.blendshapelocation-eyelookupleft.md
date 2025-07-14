

- ARKit
- ARFaceAnchor
- ARFaceAnchor.BlendShapeLocation
-  eyeLookUpLeft 

Type Property

# eyeLookUpLeft

The coefficient describing movement of the left eyelids consistent with an upward gaze.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
static let eyeLookUpLeft: ARFaceAnchor.BlendShapeLocation
```

## Discussion

The figure below shows a face geometry (see ARSCNFaceGeometry) in two states, demonstrating values of `0.0` and `1.0` for this coefficient. In both states, the values for all other ARFaceAnchor.BlendShapeLocation coefficients are set to `0.0`.

## See Also

### Left Eye

static let eyeBlinkLeft: ARFaceAnchor.BlendShapeLocation

The coefficient describing closure of the eyelids over the left eye.

static let eyeLookDownLeft: ARFaceAnchor.BlendShapeLocation

The coefficient describing movement of the left eyelids consistent with a downward gaze.

static let eyeLookInLeft: ARFaceAnchor.BlendShapeLocation

The coefficient describing movement of the left eyelids consistent with a rightward gaze.

static let eyeLookOutLeft: ARFaceAnchor.BlendShapeLocation

The coefficient describing movement of the left eyelids consistent with a leftward gaze.

static let eyeSquintLeft: ARFaceAnchor.BlendShapeLocation

The coefficient describing contraction of the face around the left eye.

static let eyeWideLeft: ARFaceAnchor.BlendShapeLocation

The coefficient describing a widening of the eyelids around the left eye.

