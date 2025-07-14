

- ARKit
- ARFaceAnchor
- ARFaceAnchor.BlendShapeLocation
-  mouthClose 

Type Property

# mouthClose

The coefficient describing closure of the lips *independent of jaw position*.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
static let mouthClose: ARFaceAnchor.BlendShapeLocation
```

## Discussion

This coefficient describes a closing of the lips without relation to the position of the jaw (the jawOpen coefficient), so some values of the mouthClose coefficient can produce unrealistic facial expressions unless other coefficients are also set to realistic values.

The figure below shows a face geometry (see ARSCNFaceGeometry) in three states:

1.  A neutral face (all ARFaceAnchor.BlendShapeLocation coefficient values at `0.0`, including both jawOpen and mouthClose)

2.  Setting only the jawOpen coefficient to `1.0`, while keeping all other coefficient values (including mouthClose) at `0.0`

3.  Setting both the jawOpen and mouthClose coefficients to `1.0`, while keeping all other coefficient values at `0.0`

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

static let mouthStretchLeft: ARFaceAnchor.BlendShapeLocation

The coefficient describing leftward movement of the left corner of the mouth.

