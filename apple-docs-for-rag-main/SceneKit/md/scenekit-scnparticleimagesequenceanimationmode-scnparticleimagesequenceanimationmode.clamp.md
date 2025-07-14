

- SceneKit
- SCNParticleImageSequenceAnimationMode
-  SCNParticleImageSequenceAnimationMode.clamp 

Case

# SCNParticleImageSequenceAnimationMode.clamp

The animation stops after displaying all of its images.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
case clamp
```

## Discussion

After animation ends, the particle continues to display the last image of the sequence. (Or the first, if the animation is playing in reverse.)

## See Also

### Constants

case `repeat`

The animation loops after displaying all of its images.

case autoReverse

After the animation displays all of its images, it plays again in reverse order.

