

- AppKit
- NSResponder
-  userActivity 

Instance Property

# userActivity

An object encapsulating a user activity supported by this responder.

macOS 10.10+

``` source
@MainActor
var userActivity: NSUserActivity? { get set }
```

## Discussion

By setting the userActivity property on a responder, the NSUserActivity object becomes managed by AppKit. You should override updateUserActivityState(_:) to write lazily any state data representing the user’s activity to the `userInfo` dictionary. AppKit automatically saves user activities it manages at appropriate times. Multiple responders can share a single NSUserActivity instance, in which case they all get a callback, such as updateUserActivityState(_:), when the system updates the user activity object.

Note

Before the update callbacks are sent, the activity object’s `userInfo` dictionary is cleared.

In macOS, NSUserActivity objects managed by NSResponder automatically becomeCurrent() based on the main window and the responder chain.

A responder object can set its userActivity property to `nil` if it no longer wants to participate. Any NSUserActivity objects that AppKit manages but have no associated responders (or documents) are automatically invalidated.

You can use this property from any thread, and it’s key-value observable (KVO).

## See Also

### Supporting User Activities

func updateUserActivityState(NSUserActivity)

Updates the state of the given user activity.

