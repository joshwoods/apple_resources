

- ARKit
- ARAnchor
-  name 

Instance Property

# name

A descriptive name for the anchor.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var name: String? { get }
```

## Mentioned in 

Managing Session Life Cycle and Tracking Quality

## Discussion

To name an anchor, create one with the init(name:transform:) initializer. This property is `nil` for anchors created otherwise.

ARKit does not display the name to users, but your app can use it to identify anchors for debugging.

## See Also

### Creating Anchors

init(transform: simd_float4x4)

Creates a new anchor object with the specified transform.

init(name: String, transform: simd_float4x4)

Creates a new anchor object with the specified transform and a descriptive name.

