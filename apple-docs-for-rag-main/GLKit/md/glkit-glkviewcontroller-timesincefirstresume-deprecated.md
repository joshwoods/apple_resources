

- GLKit
- GLKViewController
-  timeSinceFirstResume Deprecated

Instance Property

# timeSinceFirstResume

The amount of time that has passed since first time the view controller resumed sending update events.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
@MainActor
var timeSinceFirstResume: TimeInterval { get }
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## See Also

### Obtaining Information About View Updates

var framesDisplayed: Int

The number of frame updates that have been sent by the view controller since it was created.

Deprecated

var timeSinceLastResume: TimeInterval

The amount of time that has passed since the last time the view controller resumed sending update events.

Deprecated

var timeSinceLastUpdate: TimeInterval

The amount of time that has passed since the last time the view controller called the delegate’s glkViewControllerUpdate(_:) method.

Deprecated

var timeSinceLastDraw: TimeInterval

The amount of time that has passed since the last time the view controller called the view’s display() method.

Deprecated

