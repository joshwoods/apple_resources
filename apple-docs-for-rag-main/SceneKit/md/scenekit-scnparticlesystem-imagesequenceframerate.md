

- SceneKit
- SCNParticleSystem
-  imageSequenceFrameRate 

Instance Property

# imageSequenceFrameRate

The rate, in frames per second, of particle image animation. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var imageSequenceFrameRate: CGFloat { get set }
```

## Discussion

To specify a sequence of frames for animating each particle, arrange the frames as a grid in a single image, as shown in Figure 1. Then use the imageSequenceRowCount and imageSequenceColumnCount properties to specify the arrangement of frames in the images, and this property to define animation speed.

The default value is `0.0` frames per second, specifying no animation.

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

var imageSequenceFrameRateVariation: CGFloat

The range, in frames per second, of randomized frame rates for particle image animation. Animatable.

var imageSequenceAnimationMode: SCNParticleImageSequenceAnimationMode

The animation mode for particle image animation.

enum SCNParticleImageSequenceAnimationMode

Options for animating each particle with a sequence of images, used by the imageSequenceAnimationMode property.

