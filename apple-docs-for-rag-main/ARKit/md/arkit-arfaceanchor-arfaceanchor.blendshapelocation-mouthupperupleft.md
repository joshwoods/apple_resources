

- ARKit
- ARFaceAnchor
- ARFaceAnchor.BlendShapeLocation
-  mouthUpperUpLeft 

Type Property

# mouthUpperUpLeft

The coefficient describing upward movement of the upper lip on the left side.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
static let mouthUpperUpLeft: ARFaceAnchor.BlendShapeLocation
```

## Discussion

The figure below shows a face geometry (see ARSCNFaceGeometry) in two states, demonstrating values of `0.0` and `1.0` for this coefficient. In both states, the values for all other ARFaceAnchor.BlendShapeLocation coefficients are set to `0.0`.

## See Also

### Mouth and Jaw

static let jawForward: ARFaceAnchor.BlendShapeLocation

The coefficient describing forward movement of the lower jaw.

static let jawLeft: ARFaceAnchor.BlendShapeLocation

The coefficient describing leftward movement of the lower jaw.

static let jawRight: ARFaceAnchor.BlendShapeLocation

The coefficient describing rightward movement of the lower jaw.

static let jawOpen: ARFaceAnchor.BlendShapeLocation

The coefficient describing an opening of the lower jaw.

static let mouthClose: ARFaceAnchor.BlendShapeLocation

The coefficient describing closure of the lips *independent of jaw position*.

static let mouthFunnel: ARFaceAnchor.BlendShapeLocation

The coefficient describing contraction of both lips into an open shape.

static let mouthPucker: ARFaceAnchor.BlendShapeLocation

The coefficient describing contraction and compression of both closed lips.

static let mouthLeft: ARFaceAnchor.BlendShapeLocation

The coefficient describing leftward movement of both lips together.

static let mouthRight: ARFaceAnchor.BlendShapeLocation

The coefficient describing rightward movement of both lips together.

static let mouthSmileLeft: ARFaceAnchor.BlendShapeLocation

The coefficient describing upward movement of the left corner of the mouth.

static let mouthSmileRight: ARFaceAnchor.BlendShapeLocation

The coefficient describing upward movement of the right corner of the mouth.

static let mouthFrownLeft: ARFaceAnchor.BlendShapeLocation

The coefficient describing downward movement of the left corner of the mouth.

static let mouthFrownRight: ARFaceAnchor.BlendShapeLocation

The coefficient describing downward movement of the right corner of the mouth.

static let mouthDimpleLeft: ARFaceAnchor.BlendShapeLocation

The coefficient describing backward movement of the left corner of the mouth.

static let mouthDimpleRight: ARFaceAnchor.BlendShapeLocation

The coefficient describing backward movement of the right corner of the mouth.

