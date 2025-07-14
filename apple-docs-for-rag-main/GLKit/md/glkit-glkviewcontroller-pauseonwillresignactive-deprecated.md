

- GLKit
- GLKViewController
-  pauseOnWillResignActive Deprecated

Instance Property

# pauseOnWillResignActive

A Boolean value that indicates whether the view controller automatically pauses the rendering loop when the application resigns the active state.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
@MainActor
var pauseOnWillResignActive: Bool { get set }
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Discussion

The default value is true. If your application sets this to false, it must explicitly set the isPaused property to true when the application resigns the active state.

## See Also

### Controlling Frame Updates

var isPaused: Bool

A Boolean value that indicates whether the rendering loop is paused.

Deprecated

var resumeOnDidBecomeActive: Bool

A Boolean value that indicates whether the view controller automatically resumes the rendering loop when the application becomes active.

Deprecated

