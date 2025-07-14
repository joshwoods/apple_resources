

- AppKit
- NSAnimationContext
-  duration 

Instance Property

# duration

The duration used by animations created as a result of setting new values for an animatable property.

macOS 10.5+

``` source
var duration: TimeInterval { get set }
```

## Discussion

Any animations that occur as a result of setting the values of animatable properties in the current context will run for this duration.

## See Also

### Modifying the Animation Duration

var timingFunction: CAMediaTimingFunction?

The timing function used for all animations within this animation proxy group.

