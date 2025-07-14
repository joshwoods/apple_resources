

- SpriteKit
- SKView
-  delegate 

Instance Property

# delegate

A delegate that allows dynamic control of the view’s render rate.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any SKViewDelegate)? { get set }
```

## Mentioned in 

Subclassing Scenes Versus Assigning a Delegate

## See Also

### Controlling the Timing of a Scene’s Rendering

var isPaused: Bool

A Boolean value that indicates whether the view’s scene animations are paused.

var preferredFramesPerSecond: Int

The animation frame rate that the view uses to render its scene.

protocol SKViewDelegate

Methods to take custom control over the view’s render rate.

var frameInterval: Int

The number of frames that must pass before the scene is called to update its contents.

Deprecated

var preferredFrameRate: FloatDeprecated

