

- RealityKit
- AnchorEntity
-  reanchor(\_:preservingWorldTransform:) 

Instance Method

# reanchor(\_:preservingWorldTransform:)

Changes the entity’s anchoring, preserving either the world transform or the local transform.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func reanchor(
    _ target: AnchoringComponent.Target,
    preservingWorldTransform: Bool = true
)
```

## Parameters 

`target`  

Describes how the entity should be anchored in AR.

`preservingWorldTransform`  

A Boolean you set to `true` to preserve the current world space position, or `false` to use the position relative to the previous anchor for the new anchor.

## See Also

### Configuring the anchor

var anchoring: AnchoringComponent

The component that describes how the virtual content is anchored to the real world.

var anchorIdentifier: UUID?

The identifier of the AR anchor with which the anchor entity is associated, or `nil` if it isn’t currently anchored.

