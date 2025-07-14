

- AppKit
- NSDocument
-  userActivity 

Instance Property

# userActivity

An object that encapsulates a user activity the document supports.

macOS 10.10+

``` source
@MainActor
var userActivity: NSUserActivity? { get set }
```

## Discussion

NSDocument automatically creates NSUserActivity objects. The system makes user activities eligible for Handoff if the document is iCloud-based and the app’s `Info.plist` property list file includes a `CFBundleDocumentTypes` key of `NSUbiquitousDocumentUserActivityType`. The value of `NSUbiquitousDocumentUserActivityType` is a string that represents the NSUserActivity object’s activity type. The document’s URL is in the NSUserActivity object’s userInfo dictionary with the NSUserActivityDocumentURLKey.

In macOS, NSUserActivity objects that NSDocument manage automatically become current when any of the document window controller’s windows become main. Otherwise, you need to invoke becomeCurrent() at appropriate times.

AppKit automatically invalidates any NSUserActivity objects that have no associated documents or responders.

You can use this property from any thread. It’s KVO-observable in case you share the NSDocument object with other objects that need to be in sync as the document moves into and out of iCloud.

## See Also

### Related Documentation

class NSDocument

An abstract class that defines the interface for macOS documents.

### Supporting User Activities

func updateUserActivityState(NSUserActivity)

Updates the state of the given user activity.

let NSUserActivityDocumentURLKey: String

The key that identifies the document associated with a user activity.

