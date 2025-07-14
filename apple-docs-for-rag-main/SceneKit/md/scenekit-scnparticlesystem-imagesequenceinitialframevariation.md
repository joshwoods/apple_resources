

- SceneKit
- SCNParticleSystem
-  imageSequenceInitialFrameVariation 

Instance Property

# imageSequenceInitialFrameVariation

The range of randomized initial frames for particle image animation. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var imageSequenceInitialFrameVariation: CGFloat { get set }
```

## Discussion

Setting a nonzero value for this property randomizes the effect of the imageSequenceInitialFrame property. SceneKit randomly adjusts the initial animation frame for each particle by up to half the imageSequenceInitialFrameVariation value. For example, if the imageSequenceInitialFrame value is `10.0` and the imageSequenceInitialFrameVariation value is `5.0`, each particle randomly begins on a frame between frame 7.5 and frame 12.5 of the image sequence animation.

When you use image sequences for particles, SceneKit interpolates between frames of animation, so a fractional value (either for this property or for either endpoint of the range it determines) results in a partial fade between two animation frames.

The default value is `0.0` seconds, specifying no randomization.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Animating Particle Images

var imageSequenceRowCount: Int

The number of rows for treating the particle image as a grid of animation frames.

var imageSequenceColumnCount: Int

The number of columns for treating the particle image as a grid of animation frames.

var imageSequenceInitialFrame: CGFloat

The index of the first frame in a particle image animation. Animatable.

var imageSequenceFrameRate: CGFloat

The rate, in frames per second, of particle image animation. Animatable.

var imageSequenceFrameRateVariation: CGFloat

The range, in frames per second, of randomized frame rates for particle image animation. Animatable.

var imageSequenceAnimationMode: SCNParticleImageSequenceAnimationMode

The animation mode for particle image animation.

enum SCNParticleImageSequenceAnimationMode

Options for animating each particle with a sequence of images, used by the imageSequenceAnimationMode property.

