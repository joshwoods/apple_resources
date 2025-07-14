

- SceneKit
- SCNParticleSystem
-  imageSequenceAnimationMode 

Instance Property

# imageSequenceAnimationMode

The animation mode for particle image animation.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var imageSequenceAnimationMode: SCNParticleImageSequenceAnimationMode { get set }
```

## Discussion

The default value is SCNParticleImageSequenceAnimationMode.repeat, indicating that the image sequence loops continuously. For details on other values, see SCNParticleImageSequenceAnimationMode.

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

var imageSequenceFrameRateVariation: CGFloat

The range, in frames per second, of randomized frame rates for particle image animation. Animatable.

enum SCNParticleImageSequenceAnimationMode

Options for animating each particle with a sequence of images, used by the imageSequenceAnimationMode property.

