

- AppKit
- NSApplicationDelegate
-  application(\_:continue:restorationHandler:) 

Instance Method

# application(\_:continue:restorationHandler:)

Returns a Boolean value that indicates if the app successfully recreates the specified activity.

macOS 10.10+

``` source
@MainActor
optional func application(
    _ application: NSApplication,
    continue userActivity: NSUserActivity,
    restorationHandler: @escaping ([any NSUserActivityRestoring]) -> Void
) -> Bool
```

## Parameters 

`application`  

The app continuing the user activity.

`userActivity`  

The activity object containing the data associated with the task the user was performing. Use the data in this object to recreate what the user was doing.

`restorationHandler`  

A block to execute if your app creates or fetches objects to perform the task. Calling this block is optional and is only needed when specific objects are capable of continuing the activity. You can copy this block and call it at a later time. When calling a saved copy of the block, you must call it from the app’s main thread. This block has no return value and takes the following parameter:

`restorableObjects`  
An array of NSResponder or NSDocument objects that you created or fetched in order to perform the operation. The system calls the restoreUserActivityState(_:) method of each object in the array to perform the operation.

## Return Value

true if this method handled continuing the activity; false to have AppKit attempt to continue the activity.

## Discussion

The app calls this method when it receives the data associated with the user activity. Use the data stored in the `NSUserActivity` object to re-create the user’s activity. This method is your opportunity to update your app so that it can perform the associated task.

If this user activity object was created automatically by having `NSUbiquitousDocumentUserActivityType` in a `CFBundleDocumentTypes` entry, AppKit can automatically restore the NSUserActivity in macOS if this method returns false, or if it is unimplemented. It does this by creating a document of the appropriate type using the URL stored in the userInfo dictionary under the `NSUserActivityDocumentURLKey`. The system calls the NSDocument method restoreUserActivityState(_:) on the document.

## See Also

### Continuing User Activities

func application(NSApplication, willContinueUserActivityWithType: String) -> Bool

Returns a Boolean value that indicates if the app can continue the specified activity.

func application(NSApplication, didFailToContinueUserActivityWithType: String, error: any Error)

Tells the delegate that the app couldn’t continue the specified activity.

func application(NSApplication, didUpdate: NSUserActivity)

Tells the delegate that there are changes to the specified activity.

