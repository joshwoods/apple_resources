

- RealityKit
- AnimationDefinition
-  blendLayer 

Instance Property

# blendLayer

The order in which the framework composites the animation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var blendLayer: Int32 { get set }
```

**Required**

## Discussion

The framework applies multiple animations on the same target in ascending order of this property’s value. Animations in a lower layer run before animations in a higher layer. Animations that share the same value apply in the order that they execute.

## See Also

### Configuring the animation

var name: String

A textual name for the animation.

**Required**

var bindTarget: BindTarget

A textual name that identifies the particular property that animates.

**Required**

