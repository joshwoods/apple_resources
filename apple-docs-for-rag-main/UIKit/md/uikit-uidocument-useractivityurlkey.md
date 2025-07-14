

- UIKit
- UIDocument
-  userActivityURLKey 

Type Property

# userActivityURLKey

The key that identifies the document associated with a user activity.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class let userActivityURLKey: String
```

## Discussion

You use this key in the userInfo dictionary of an NSUserActivity object. Its value is the URL of the document associated with the user activity.

When the `NSUbiquitousDocumentUserActivityType` key is present in a CFBundleDocumentTypes entry, AppKit automatically creates an NSUserActivity object for documents in iCloud, using the given activity type.

## See Also

### Constants

enum ChangeKind

Constants that specify the kind of change to a document.

enum SaveOperation

Constants that specify the type of save operation.

struct State

Constants that specify the document state.

