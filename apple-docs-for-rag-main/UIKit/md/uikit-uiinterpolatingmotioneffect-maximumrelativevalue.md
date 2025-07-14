

- UIKit
- UIInterpolatingMotionEffect
-  maximumRelativeValue 

Instance Property

# maximumRelativeValue

The value that maps to the maximum viewer offset.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var maximumRelativeValue: Any? { get set }
```

## Discussion

The value in this property is the value returned when the viewer offset value along the given axis is 1.

## See Also

### Accessing the motion attributes

var keyPath: String

The key path you want to modify on the view.

var type: UIInterpolatingMotionEffect.EffectType

The tilt direction to monitor.

var minimumRelativeValue: Any?

The value that maps to the minimum viewer offset.

