

- UIKit
- UIDocument
-  updateUserActivityState(\_:) 

Instance Method

# updateUserActivityState(\_:)

Updates the state of the given user activity.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func updateUserActivityState(_ userActivity: NSUserActivity)
```

## Parameters 

`userActivity`  

The user activity to be updated.

## Discussion

The default implementation of this method puts the document’s fileURL into the NSUserActivity object’s userInfo dictionary with the userActivityURLKey. UIDocument automatically sets the needsSave property of the NSUserActivity object to true when the fileURL changes.

## See Also

### Supporting user activities

var userActivity: NSUserActivity?

An object encapsulating a user activity supported by this document.

func restoreUserActivityState(NSUserActivity)

Restores the state needed to continue the given user activity.

