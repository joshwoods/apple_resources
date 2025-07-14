

- UIKit
- UIPasteboard
-  removedNotification 

Type Property

# removedNotification

A notification that a pasteboard object posts just before an app removes it.

iOSiPadOSMac CatalystvisionOS

``` source
nonisolated
class let removedNotification: NSNotification.Name
```

## Discussion

The removal class method is remove(withName:). There is no `userInfo` dictionary.

## See Also

### Notifications

class let changedNotification: NSNotification.Name

A notification that a pasteboard object posts when its contents change.

