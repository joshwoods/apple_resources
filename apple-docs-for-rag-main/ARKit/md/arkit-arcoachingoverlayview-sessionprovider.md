

- ARKit
- ARCoachingOverlayView
-  sessionProvider 

Instance Property

# sessionProvider

An object you designate that provides the current session.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
@IBOutlet @MainActor
weak var sessionProvider: (any ARSessionProviding)? { get set }
```

## Discussion

Use this property to set the coaching overlay’s session when loading from a storyboard. If you set this property at runtime, the coaching overlay keeps its session property up to date for you. If your app recreates its ARSession at any point, you may find it convienient to set the sessionProvider once rather than update the coaching overlay’s session manually.

## See Also

### Providing the Session

var session: ARSession?

The session this view uses to provide coaching.

