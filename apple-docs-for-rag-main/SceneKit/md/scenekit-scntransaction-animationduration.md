

- SceneKit
- SCNTransaction
-  animationDuration 

Type Property

# animationDuration

Returns the duration, in seconds, of all animations within the current transaction.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class var animationDuration: CFTimeInterval { get set }
```

## Return Value

The animation duration, in seconds.

## Mentioned in 

Animating SceneKit Content

## Discussion

The default duration is zero for transactions automatically created by SceneKit, and `0.25` for animations you create using the begin() method.

## See Also

### Overriding Animation Duration and Timing

class var animationTimingFunction: CAMediaTimingFunction?

Returns the timing function that SceneKit uses for all animations within this transaction group.

