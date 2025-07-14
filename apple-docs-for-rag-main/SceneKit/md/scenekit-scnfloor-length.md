

- SceneKit
- SCNFloor
-  length 

Instance Property

# length

The extent of the floor along its z-axis. Animatable.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var length: CGFloat { get set }
```

## Discussion

The floor is centered in its local coordinate system. For example, a floor of length `10.0` extends from `-5.0` to `5.0` along the z-axis. The default width is zero, indicating that the floor’s length is infinite.

You can animate changes to this property’s value. See `Animating SceneKit Content`.

## See Also

### Adjusting a Floor’s Size

var width: CGFloat

The extent of the floor along its x-axis. Animatable.

