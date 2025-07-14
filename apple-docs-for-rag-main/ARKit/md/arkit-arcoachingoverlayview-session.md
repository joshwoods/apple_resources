

- ARKit
- ARCoachingOverlayView
-  session 

Instance Property

# session

The session this view uses to provide coaching.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
@MainActor
var session: ARSession? { get set }
```

## Discussion

The coaching overlay monitors your app’s ARSession and reacts according to its tracking status. You don’t need to set this property if you set sessionProvider instead.

## See Also

### Providing the Session

var sessionProvider: (any ARSessionProviding)?

An object you designate that provides the current session.

