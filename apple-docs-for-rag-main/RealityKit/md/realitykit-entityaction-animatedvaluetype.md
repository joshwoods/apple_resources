

- RealityKit
- EntityAction
-  animatedValueType 

Instance Property

# animatedValueType

A value that defines the type that the action animates, if the action animates a target value.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var animatedValueType: (any AnimatableData.Type)? { get }
```

**Required**

## Discussion

In your implementation, return a type that matches the action animation’s bind target.

For example if the action animates a Transform, return `Transform.self` in your implementation, and set the action animation’s bind target to BindTarget.transform when creating an AnimationResource with `AnimationResource.makeActionAnimation(...)`.

