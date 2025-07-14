

- RealityKit
- ModelComponent
-  materials 

Instance Property

# materials

The materials that define the model’s visual appearance.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
var materials: [any Material]
```

## Discussion

Each MeshResource requires a set of materials. An entity that has no materials renders using a magenta striped material. To determine the number of materials a mesh requires, use expectedMaterialCount.

