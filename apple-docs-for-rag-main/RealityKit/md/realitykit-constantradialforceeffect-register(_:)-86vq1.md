

- RealityKit
- ConstantRadialForceEffect
-  register(\_:) 

Type Method

# register(\_:)

Registers the custom effect.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor @preconcurrency
static func register(_ updateHandler: (@MainActor (inout ForceEffectEvent) -> Void)? = nil)
```

## Parameters 

`updateHandler`  

A closure that computes custom forces for rigid bodies.

## Discussion

If a handler is specified, the physics system calls the handler and ignores the update function.

