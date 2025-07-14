

- SceneKit
- SCNMorpher
-  targets 

Instance Property

# targets

The array of target geometries to morph between.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
var targets: [SCNGeometry] { get set }
```

## Discussion

An array of SCNGeometry objects.

A morpher blends between a base geometry, specified in the geometry property of the node the morpher is attached to, and one or more target geometries. The base geometry and all target geometries must be topologically identical—that is, they must contain the same number and structural arrangement of vertices.

