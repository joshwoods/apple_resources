

- ARKit
- ARAnchor
-  init(name:transform:) 

Initializer

# init(name:transform:)

Creates a new anchor object with the specified transform and a descriptive name.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
init(
    name: String,
    transform: simd_float4x4
)
```

## Parameters 

`name`  

A descriptive name for the anchor. ARKit does not display the name to users, but your app can use it to identify anchors for debugging.

`transform`  

A matrix encoding the position, orientation, and scale of the anchor relative to the world coordinate space of the AR session the anchor is placed in.

## Discussion

World coordinate space in ARKit always follows a right-handed convention, but is oriented based on the session configuration. For details, see Understanding World Tracking.

## Discussion

Use the add(anchor:) method to begin tracking your custom anchor in an AR session.

## See Also

### Creating Anchors

init(transform: simd_float4x4)

Creates a new anchor object with the specified transform.

var name: String?

A descriptive name for the anchor.

