

- SceneKit
- SCNParticleSystem
-  imageSequenceFrameRateVariation 

Instance Property

# imageSequenceFrameRateVariation

The range, in frames per second, of randomized frame rates for particle image animation. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var imageSequenceFrameRateVariation: CGFloat { get set }
```

## Discussion

Setting a nonzero value for this property randomizes the effect of the imageSequenceFrameRate property. SceneKit randomly adjusts the animation speed for each particle by up to half the imageSequenceFrameRateVariation value. For example, if the imageSequenceFrameRate value is `10.0` frames per second and the imageSequenceFrameRateVariation value is `10.0` seconds, each particle animates at a random rate between `5.0` and `15.0` frames per second.

The default value is `0.0` frames per second, specifying no randomization.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Animating Particle Images

var imageSequenceRowCount: Int

The number of rows for treating the particle image as a grid of animation frames.

var imageSequenceColumnCount: Int

The number of columns for treating the particle image as a grid of animation frames.

var imageSequenceInitialFrame: CGFloat

The index of the first frame in a particle image animation. Animatable.

var imageSequenceInitialFrameVariation: CGFloat

The range of randomized initial frames for particle image animation. Animatable.

var imageSequenceFrameRate: CGFloat

The rate, in frames per second, of particle image animation. Animatable.

var imageSequenceAnimationMode: SCNParticleImageSequenceAnimationMode

The animation mode for particle image animation.

enum SCNParticleImageSequenceAnimationMode

Options for animating each particle with a sequence of images, used by the imageSequenceAnimationMode property.

