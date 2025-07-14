

- SceneKit
- SCNSkinner
-  baseGeometry 

Instance Property

# baseGeometry

The geometry whose surface the skinner’s animation skeleton deforms.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
var baseGeometry: SCNGeometry? { get set }
```

## Discussion

Use this property to:

- Change the appearance of a skinned model using the geometry’s materials.

- Replace the skinner’s geometry with a different model. The new model must be compatible with the skinner’s animation skeleton (that is, it must have the same number of vertices).

Because multiple skinner objects can reference the same geometry, you can use the geometry with several nodes in your scene, each with a different skinner object to pose the model in different ways.

## See Also

### Working with a Skinned Geometry

var baseGeometryBindTransform: SCNMatrix4

The coordinate transformation for the skinner’s geometry in its default state.

