

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Configuration
-  meshPrimitive 

Instance Property

# meshPrimitive

On macOS, this property can be used to change the output geometry mesh primitive for all output geometry in the session, regardless of `Detail` setting. This will also change the mesh primitives in both OBJ and USD outputs. By default, triangle meshes are created.

Mac Catalyst 18.0+macOS 15.0+

``` source
var meshPrimitive: PhotogrammetrySession.Configuration.MeshPrimitive
```

