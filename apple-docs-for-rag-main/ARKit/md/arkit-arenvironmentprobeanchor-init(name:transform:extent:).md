

- ARKit
- AREnvironmentProbeAnchor
-  init(name:transform:extent:) 

Initializer

# init(name:transform:extent:)

Creates a new anchor object with a descriptive name.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
init(
    name: String,
    transform: simd_float4x4,
    extent: simd_float3
)
```

## Parameters 

`name`  

A descriptive name for the anchor. ARKit doesn’t display the name to users, but your app can use it to identify anchors for debugging.

`transform`  

A matrix that encodes the position, orientation, and scale of the anchor, relative to the world coordinate space of the AR session in which you place the anchor.

World coordinate space in ARKit always follows a right-handed convention, but is oriented based on the session configuration. For details, see Understanding World Tracking.

`extent`  

The area around the anchor’s position that contains the textrure.

An environment probe anchor may have an infinite extent, which indicates that its texture is a global lighting environment, or a finite extent, which indicates that its texture represents the local lighting conditions in a specific area of the scene.

## Discussion

Use the add(anchor:) method to begin tracking your custom anchor in an AR session. After you add an environment probe anchor to the scene, ARKit begins generating environment textures for it. To be notified when the anchor has a new environmentTexture, implement the session(_:didUpdate:), renderer(_:didUpdate:for:), or view(_:didUpdate:for:) delegate method.

## See Also

### Creating Probe Anchors

init(transform: simd_float4x4, extent: simd_float3)

Creates a new environment probe anchor.

