

- RealityKit
- MeshResource
- MeshResource.Part
-  jointInfluences 

Instance Property

# jointInfluences

A buffer of vertex-joint influences which defines how the mesh deforms in response to the skeleton that it is bound to. Each vertex may be influenced by one or more joints defined by the skeleton.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
var jointInfluences: MeshResource.JointInfluences? { get set }
```

