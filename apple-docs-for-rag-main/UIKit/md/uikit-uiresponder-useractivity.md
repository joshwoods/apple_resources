

- UIKit
- UIResponder
-  userActivity 

Instance Property

# userActivity

An object encapsulating a user activity supported by this responder.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var userActivity: NSUserActivity? { get set }
```

## Discussion

By setting the userActivity property on a responder, the NSUserActivity object becomes managed by UIKit. User activities managed by UIKit are saved automatically at appropriate times. You can lazily add state data representing the user’s activity using the updateUserActivityState(_:) override. Multiple responders can share a single NSUserActivity instance, in which case they all get an updateUserActivityState(_:) callback.

Note

Prior to invoking updateUserActivityState(_:) on all of the associated objects, the `userInfo` dictionary for the NSUserActivity object is cleared.

A responder object can set its userActivity property to `nil` if it no longer wants to participate. Any NSUserActivity objects that are managed by UIKit but which have no associated responders (or documents) are automatically invalidated.

## See Also

### Supporting user activities

func restoreUserActivityState(NSUserActivity)

Restores the state needed to continue the given user activity.

func updateUserActivityState(NSUserActivity)

Updates the state of the given user activity.

