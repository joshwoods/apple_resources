

- RealityKit
- HasAnchoring
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

