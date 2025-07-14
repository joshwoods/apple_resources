

- AppKit
- NSAnimationContext
-  timingFunction 

Instance Property

# timingFunction

The timing function used for all animations within this animation proxy group.

macOS 10.7+

``` source
var timingFunction: CAMediaTimingFunction? { get set }
```

## Discussion

The NSAnimationContext timing function is analogous to the CATransaction setAnimationTimingFunction(_:) method.

Animations initiated through the “animator” proxy syntax, that do not have an explicitly specified timing functions, will inherit the enclosing `NSAnimationContext` instance’s timingFunction if it is not `nil` (which is the default).

As with the existing duration property, changing a timing function causes the same change in the underlying CATransaction instance’s animationTimingFunction().

Also as with the duration property, you may change the timingFunction any number of times within a given NSAnimationContext beginGrouping() and endGrouping() block. Changes to the `timingFunction` will apply to any animations that are subsequently initiated in that NSAnimationContext grouping, until the `timingFunction` is possibly changed again.

## See Also

### Modifying the Animation Duration

var duration: TimeInterval

The duration used by animations created as a result of setting new values for an animatable property.

