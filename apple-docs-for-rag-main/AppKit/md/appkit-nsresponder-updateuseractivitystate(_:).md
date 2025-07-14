

- AppKit
- NSResponder
-  updateUserActivityState(\_:) 

Instance Method

# updateUserActivityState(\_:)

Updates the state of the given user activity.

macOS 10.10+

``` source
@MainActor
func updateUserActivityState(_ userActivity: NSUserActivity)
```

## Parameters 

`userActivity`  

The user activity to be updated.

## Discussion

Subclasses override this method to update the state of the supplied `userActivity`. Add state representing the user’s activity into `userActivity` using its addUserInfoEntries(from:) method. When the state is dirty, set the needsSave property to true.

When an NSUserActivity object managed by AppKit is updated, an empty `userInfo` dictionary is given to the user activity, and all of the objects associated with the user activity are sent an NSResponder message.

## See Also

### Related Documentation

class NSResponder

An abstract class that forms the basis of event and command processing in AppKit.

### Supporting User Activities

var userActivity: NSUserActivity?

An object encapsulating a user activity supported by this responder.

