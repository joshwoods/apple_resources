

- SceneKit
- SCNTransaction
-  animationTimingFunction 

Type Property

# animationTimingFunction

Returns the timing function that SceneKit uses for all animations within this transaction group.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
@NSCopying
class var animationTimingFunction: CAMediaTimingFunction? { get set }
```

## Return Value

The media timing function for the transaction’s animations.

## Discussion

Media timing functions, also known as *animation curves*, define the relationship between the elapsed time of an animation and its effect on a property. For example, the easeInEaseOut function creates an effect that begins slowly, speeds up, and then finishes slowly.

## See Also

### Overriding Animation Duration and Timing

class var animationDuration: CFTimeInterval

Returns the duration, in seconds, of all animations within the current transaction.

