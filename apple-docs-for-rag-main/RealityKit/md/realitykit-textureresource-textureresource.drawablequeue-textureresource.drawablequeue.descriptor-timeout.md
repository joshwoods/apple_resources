

- RealityKit
- TextureResource
- TextureResource.DrawableQueue
- TextureResource.DrawableQueue.Descriptor
-  timeout 

Instance Property

# timeout

Specifies a timeout value in seconds when querying nextDrawable(). nextDrawable() will be blocked for up to the specified timeout period for a drawable to become available else throws `NextDrawableError.timeoutReached`. By default this is set to 1 second. Note that if `allowsNextDrawableTimeout` is false, then the timeout parameter will be ignored.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var timeout: Duration { get set }
```

