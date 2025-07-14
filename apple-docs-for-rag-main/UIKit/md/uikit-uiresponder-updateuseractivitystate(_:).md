

- UIKit
- UIResponder
-  updateUserActivityState(\_:) 

Instance Method

# updateUserActivityState(\_:)

Updates the state of the given user activity.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func updateUserActivityState(_ activity: NSUserActivity)
```

## Parameters 

`activity`  

The user activity to be updated.

## Discussion

Subclasses override this method to update the state of the given user activity. You should add state representing the user’s activity into the NSUserActivity object using its addUserInfoEntries(from:) method. When the state is dirty, you should set the needsSave property of the NSUserActivity to true, and this method will be called at an appropriate time.

When an NSUserActivity object managed by UIKit is updated, an empty `userInfo` dictionary is given to the NSUserActivity object, and all of the objects associated with the NSUserActivity are then sent an updateUserActivityState(_:) message.

## See Also

### Supporting user activities

var userActivity: NSUserActivity?

An object encapsulating a user activity supported by this responder.

func restoreUserActivityState(NSUserActivity)

Restores the state needed to continue the given user activity.

