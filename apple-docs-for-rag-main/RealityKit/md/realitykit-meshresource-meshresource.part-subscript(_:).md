

- RealityKit
- MeshResource
- MeshResource.Part
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

The buffer for a given semantic. There can only be one buffer for any given ID.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
subscript(semantic: S) -> MeshBuffer? where S : MeshBufferSemantic { get set }
```

