

- ARKit
- PlaneAnchor
-  alignment 

Instance Property

# alignment

The general orientation of the detected plane with respect to gravity.

visionOS 1.0+

``` source
var alignment: PlaneAnchor.Alignment { get }
```

## See Also

### Inspecting a plane anchor

var originFromAnchorTransform: simd_float4x4

The location and orientation of a plane in world space.

enum Alignment

Values describing possible general orientations of a detected plane with respect to gravity.

var classification: PlaneAnchor.Classification

Get the classification of this plane.

enum Classification

The kinds of object classification a plane anchor can have.

var description: String

A textual representation of this anchor.

