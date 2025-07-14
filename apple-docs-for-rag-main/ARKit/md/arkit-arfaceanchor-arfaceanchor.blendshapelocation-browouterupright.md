

- ARKit
- ARFaceAnchor
- ARFaceAnchor.BlendShapeLocation
-  browOuterUpRight 

Type Property

# browOuterUpRight

The coefficient describing upward movement of the outer portion of the right eyebrow.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
static let browOuterUpRight: ARFaceAnchor.BlendShapeLocation
```

## Discussion

The figure below shows a face geometry (see ARSCNFaceGeometry) in two states, demonstrating values of `0.0` and `1.0` for this coefficient. In both states, the values for all other ARFaceAnchor.BlendShapeLocation coefficients are set to `0.0`.

## See Also

### Eyebrows, Cheeks, and Nose

static let browDownLeft: ARFaceAnchor.BlendShapeLocation

The coefficient describing downward movement of the outer portion of the left eyebrow.

static let browDownRight: ARFaceAnchor.BlendShapeLocation

The coefficient describing downward movement of the outer portion of the right eyebrow.

static let browInnerUp: ARFaceAnchor.BlendShapeLocation

The coefficient describing upward movement of the inner portion of both eyebrows.

static let browOuterUpLeft: ARFaceAnchor.BlendShapeLocation

The coefficient describing upward movement of the outer portion of the left eyebrow.

static let cheekPuff: ARFaceAnchor.BlendShapeLocation

The coefficient describing outward movement of both cheeks.

static let cheekSquintLeft: ARFaceAnchor.BlendShapeLocation

The coefficient describing upward movement of the cheek around and below the left eye.

static let cheekSquintRight: ARFaceAnchor.BlendShapeLocation

The coefficient describing upward movement of the cheek around and below the right eye.

static let noseSneerLeft: ARFaceAnchor.BlendShapeLocation

The coefficient describing a raising of the left side of the nose around the nostril.

static let noseSneerRight: ARFaceAnchor.BlendShapeLocation

The coefficient describing a raising of the right side of the nose around the nostril.

