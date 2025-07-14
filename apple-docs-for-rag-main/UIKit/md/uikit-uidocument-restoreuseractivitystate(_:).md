

- UIKit
- UIDocument
-  restoreUserActivityState(\_:) 

Instance Method

# restoreUserActivityState(\_:)

Restores the state needed to continue the given user activity.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func restoreUserActivityState(_ userActivity: NSUserActivity)
```

## Parameters 

`userActivity`  

The user activity to be continued.

## Discussion

Subclasses override this method to restore the responder’s state with the given user activity. The override should use the state data contained in the `userInfo` dictionary of the given user activity to restore the object.

User activities managed by NSDocument can be restored automatically, if false is returned from `application:continueActivity:restorationHandler:` or if it’s unimplemented. In this situation, the document is opened by the NSDocumentController method openDocument(withContentsOf:display:completionHandler:) and receives a restoreUserActivityState(_:) message.

## See Also

### Supporting user activities

var userActivity: NSUserActivity?

An object encapsulating a user activity supported by this document.

func updateUserActivityState(NSUserActivity)

Updates the state of the given user activity.

