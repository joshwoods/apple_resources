

- SceneKit
- SCNSkinner
-  baseGeometryBindTransform 

Instance Property

# baseGeometryBindTransform

The coordinate transformation for the skinner’s geometry in its default state.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
var baseGeometryBindTransform: SCNMatrix4 { get set }
```

**macOS**

``` source
var baseGeometryBindTransform: SCNMatrix4 { get set }
```

## Discussion

This transformation matrix converts from the geometry’s model coordinate space to that used by the animation skeleton. It should match the coordinate space in which the skeleton (the nodes in the bones array) is initially defined, binding the model to its default pose.

The default value is SCNMatrix4Identity.

## See Also

### Working with a Skinned Geometry

var baseGeometry: SCNGeometry?

The geometry whose surface the skinner’s animation skeleton deforms.

