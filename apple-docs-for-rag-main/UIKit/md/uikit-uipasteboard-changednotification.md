

- UIKit
- UIPasteboard
-  changedNotification 

Type Property

# changedNotification

A notification that a pasteboard object posts when its contents change.

iOSiPadOSMac CatalystvisionOS

``` source
nonisolated
class let changedNotification: NSNotification.Name
```

## Discussion

This happens at the same time the pasteboard’s change count (changeCount property) is incremented. Changes include the addition, removal, and modification of pasteboard items. The `userInfo` dictionary may contain the representation types of pasteboard items that have been added to or removed from the pasteboard. See UserInfo Dictionary Keys for the keys used to access these representation types. If pasteboard items have been modified but not added or removed, the `userInfo` dictionary is `nil`.

## See Also

### Notifications

class let removedNotification: NSNotification.Name

A notification that a pasteboard object posts just before an app removes it.

