

- SpriteKit
- SKView
-  preferredFrameRate Deprecated

Instance Property

# preferredFrameRate

iOS 10.0–10.0DeprecatediPadOS 10.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.12DeprecatedtvOS 10.0–10.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
var preferredFrameRate: Float { get set }
```

## Discussion

This function is deprecated. Use preferredFramesPerSecond instead.

## See Also

### Controlling the Timing of a Scene’s Rendering

var isPaused: Bool

A Boolean value that indicates whether the view’s scene animations are paused.

var preferredFramesPerSecond: Int

The animation frame rate that the view uses to render its scene.

var delegate: (any SKViewDelegate)?

A delegate that allows dynamic control of the view’s render rate.

protocol SKViewDelegate

Methods to take custom control over the view’s render rate.

var frameInterval: Int

The number of frames that must pass before the scene is called to update its contents.

Deprecated

