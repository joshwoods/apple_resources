

- SceneKit
- SCNTransaction
-  disableActions 

Type Property

# disableActions

Returns a Boolean value indicating whether changes to animatable properties during the transaction are implicitly animated.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class var disableActions: Bool { get set }
```

## Return Value

true if implicit animation is disabled; false if implicit animation is allowed.

## Discussion

By default (when this property is false), any changes to animatable properties of objects in the scene graph implicitly create animations. (These animations may not be visible unless you use the animationDuration property to set a nonzero duration for the transaction.) Set this property to true to disable implicit animation during the transaction.

Disabling animation applies to all property changes in the current transaction and any nested transactions within it. However, you can use this property again within a nested transaction to enable implicit animation for that transaction.

