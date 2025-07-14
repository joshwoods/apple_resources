

- RealityKit
- BindableValue
-  value 

Instance Property

# value

The main accessor for the bind value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var value: T { get set }
```

## Discussion

This property returns the animated value (animatedValue) if an animation is active. Otherwise, this property returns the base value (baseValue).

When you assign a value to this property, the setter assigns the value you provide to baseValue.

## See Also

### Accessing the value

var baseValue: T

A value that reflects the state of the animated property before or after an animation.

var animatedValue: T?

A value that represents the state of the animated property as an animation progresses.

