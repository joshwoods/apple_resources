

- SpriteKit
- SKView
-  frameInterval Deprecated

Instance Property

# frameInterval

The number of frames that must pass before the scene is called to update its contents.

iOS 7.0–10.0DeprecatediPadOS 7.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.12DeprecatedtvOSDeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
var frameInterval: Int { get set }
```

## Discussion

The default value is `1`, which results in your game being notified at the refresh rate of the display. If the value is set to a value larger than `1`, the display link notifies your game at a fraction of the native refresh rate. For example, setting the interval to `2` causes the scene to be called every other frame, providing half the frame rate.

Behavior is undefined with a value less than `1`.

This property is deprecated. Use preferredFramesPerSecond, or view(_:shouldRenderAtTime:) instead.

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

var preferredFrameRate: FloatDeprecated

