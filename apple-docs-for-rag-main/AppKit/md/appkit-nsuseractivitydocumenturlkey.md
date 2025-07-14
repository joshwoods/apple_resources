

- AppKit
-  NSUserActivityDocumentURLKey 

Global Variable

# NSUserActivityDocumentURLKey

The key that identifies the document associated with a user activity.

macOS 10.10+

``` source
let NSUserActivityDocumentURLKey: String
```

## Discussion

You use this key in the userInfo dictionary of an NSUserActivity object. Its value is the URL of the document associated with the user activity.

When the `NSUbiquitousDocumentUserActivityType` key is present in a CFBundleDocumentTypes entry, AppKit automatically creates an NSUserActivity object for documents in iCloud, using the given activity type.

## See Also

### Supporting User Activities

var userActivity: NSUserActivity?

An object that encapsulates a user activity the document supports.

func updateUserActivityState(NSUserActivity)

Updates the state of the given user activity.

