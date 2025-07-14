

- GLKit
- GLKViewController
-  framesPerSecond Deprecated

Instance Property

# framesPerSecond

The actual rate that the view controller attempts to call the view to update its contents.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
@MainActor
var framesPerSecond: Int { get }
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Discussion

The view controller attempts to maintain this frame rate, but it may still drop frames if the per-frame processing performed by your application takes more time than the time between frames.

## See Also

### Configuring the Frame rate

var preferredFramesPerSecond: Int

The rate you want the view controller to call the view to update the contents of the view.

Deprecated

