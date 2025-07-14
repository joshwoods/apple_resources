

- RealityKit
- OrbitEntityAction
-  animatedValueType 

Instance Property

# animatedValueType

The type for the value that the action modifies over time.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var animatedValueType: (any AnimatableData.Type)? { get }
```

## Discussion

Set to `nil` for an action that doesn’t modify a value.

