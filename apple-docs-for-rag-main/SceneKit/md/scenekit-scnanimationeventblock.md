

- SceneKit
-  SCNAnimationEventBlock 

Type Alias

# SCNAnimationEventBlock

Signature for the block called when an animation event triggers.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias SCNAnimationEventBlock = (any SCNAnimationProtocol, Any, Bool) -> Void
```

## Discussion

The block takes the following parameters:

animation  
The animation triggering the animation event.

animatedObject  
The Scene Kit object affected by the animation.

playingBackward  
true if the animation is playing in reverse; otherwise, false.

