

- ARKit
- AREnvironmentProbeAnchor
-  init(transform:extent:) 

Initializer

# init(transform:extent:)

Creates a new environment probe anchor.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
init(
    transform: simd_float4x4,
    extent: simd_float3
)
```

## Parameters 

`transform`  

A matrix that encodes the position, orientation, and scale of the anchor, relative to the world coordinate space of the AR session in which you place the anchor.

`extent`  

The extent (of *bounds*) of the probe anchor.

World coordinate space in ARKit always follows a right-handed convention, but is oriented based on the session configuration. For details, see Understanding World Tracking.

## Discussion

Use the add(anchor:) method to begin tracking your custom anchor in an AR session. After you add an environment probe anchor to the scene, ARKit begins generating environment textures for it. To be notified when the anchor has a new environmentTexture, implement the session(_:didUpdate:), renderer(_:didUpdate:for:), or view(_:didUpdate:for:) delegate method.

## See Also

### Creating Probe Anchors

init(name: String, transform: simd_float4x4, extent: simd_float3)

Creates a new anchor object with a descriptive name.

