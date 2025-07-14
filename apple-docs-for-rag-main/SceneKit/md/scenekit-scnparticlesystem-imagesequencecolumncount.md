

- SceneKit
- SCNParticleSystem
-  imageSequenceColumnCount 

Instance Property

# imageSequenceColumnCount

The number of columns for treating the particle image as a grid of animation frames.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var imageSequenceColumnCount: Int { get set }
```

## Discussion

To specify a sequence of frames for animating each particle, arrange the frames as a grid in a single image, as shown in Figure 1. Then use this property and the imageSequenceRowCount property to specify the arrangement of frames in the image, and the imageSequenceInitialFrame and imageSequenceFrameRate properties to define animation timing.

The default value is `1`. If the imageSequenceRowCount value is also `1` (the default), this specifies no animation for particle images.

## See Also

### Animating Particle Images

var imageSequenceRowCount: Int

The number of rows for treating the particle image as a grid of animation frames.

var imageSequenceInitialFrame: CGFloat

The index of the first frame in a particle image animation. Animatable.

var imageSequenceInitialFrameVariation: CGFloat

The range of randomized initial frames for particle image animation. Animatable.

var imageSequenceFrameRate: CGFloat

The rate, in frames per second, of particle image animation. Animatable.

var imageSequenceFrameRateVariation: CGFloat

The range, in frames per second, of randomized frame rates for particle image animation. Animatable.

var imageSequenceAnimationMode: SCNParticleImageSequenceAnimationMode

The animation mode for particle image animation.

enum SCNParticleImageSequenceAnimationMode

Options for animating each particle with a sequence of images, used by the imageSequenceAnimationMode property.

