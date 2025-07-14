

- UIKit
- UIDocument
-  userActivity 

Instance Property

# userActivity

An object encapsulating a user activity supported by this document.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var userActivity: NSUserActivity? { get set }
```

## Discussion

UIDocument automatically creates NSUserActivity objects. The system makes user activities eligible for Handoff if the document is iCloud-based and the app’s `Info.plist` property list file includes a CFBundleDocumentTypes key of `NSUbiquitousDocumentUserActivityType`. The value of `NSUbiquitousDocumentUserActivityType` is a string that represents the NSUserActivity object’s activity type. The document’s URL is in the NSUserActivity object’s userInfo dictionary with the userActivityURLKey.

In iOS, to make an NSUserActivity object that UIKit manages current, you must either call becomeCurrent() explicitly or have the document’s NSUserActivity object also set on a UIViewController object that’s in the view hierarchy when the app comes to the foreground.

You can use this property from any thread. It’s KVO-observable in case you share the userActivity object with other objects that need to be kept in sync as the document moves into and out of iCloud.

## See Also

### Supporting user activities

func restoreUserActivityState(NSUserActivity)

Restores the state needed to continue the given user activity.

func updateUserActivityState(NSUserActivity)

Updates the state of the given user activity.

