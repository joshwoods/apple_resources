

- RealityKit
- MeshResource
- MeshResource.JointInfluences
-  init(influences:influencesPerVertex:) 

Initializer

# init(influences:influencesPerVertex:)

Associates every vertex in the mesh with a fixed number of influences per vertex.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
init(
    influences: MeshBuffers.JointInfluences,
    influencesPerVertex: Int
)
```

## Parameters 

`influences`  

Buffer of joint influences.

`influencesPerVertex`  

The number of consecutive influences used by each vertex.

## Discussion

Note

The buffer should contain `vertexCount * influencesPerVertex` elements.

