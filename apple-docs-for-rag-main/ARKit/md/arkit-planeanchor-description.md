

- ARKit
- PlaneAnchor
-  description 

Instance Property

# description

A textual representation of this anchor.

visionOS 1.0+

``` source
var description: String { get }
```

## See Also

### Inspecting a plane anchor

var originFromAnchorTransform: simd_float4x4

The location and orientation of a plane in world space.

var alignment: PlaneAnchor.Alignment

The general orientation of the detected plane with respect to gravity.

enum Alignment

Values describing possible general orientations of a detected plane with respect to gravity.

var classification: PlaneAnchor.Classification

Get the classification of this plane.

enum Classification

The kinds of object classification a plane anchor can have.

