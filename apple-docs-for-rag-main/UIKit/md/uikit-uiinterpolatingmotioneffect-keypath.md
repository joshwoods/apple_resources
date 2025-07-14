

- UIKit
- UIInterpolatingMotionEffect
-  keyPath 

Instance Property

# keyPath

The key path you want to modify on the view.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var keyPath: String { get }
```

## Discussion

This property must correspond to an animatable property of the view to which the motion effect is attached.

## See Also

### Accessing the motion attributes

var type: UIInterpolatingMotionEffect.EffectType

The tilt direction to monitor.

var minimumRelativeValue: Any?

The value that maps to the minimum viewer offset.

var maximumRelativeValue: Any?

The value that maps to the maximum viewer offset.

