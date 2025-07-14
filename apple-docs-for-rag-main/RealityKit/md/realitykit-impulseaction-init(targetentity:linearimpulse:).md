

- RealityKit
- ImpulseAction
-  init(targetEntity:linearImpulse:) 

Initializer

# init(targetEntity:linearImpulse:)

Creates a new impulse action.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    targetEntity: ActionEntityResolution = .sourceEntity,
    linearImpulse: SIMD3 = [0, 1, 0]
)
```

## Parameters 

`targetEntity`  

The entity that the impulse acts upon.

`linearImpulse`  

The impulse in newton seconds (in physics simulation space).

