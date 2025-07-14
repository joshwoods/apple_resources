

- UIKit
- NSTextStorage
-  didProcessEditingNotification 

Type Property

# didProcessEditingNotification

A notification that posts after a text storage finishes processing edits.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
class let didProcessEditingNotification: NSNotification.Name
```

## Discussion

The framework posts this notification after a text storage finishes processing edits in processEditing(). Observers other than the delegate shouldn’t make further changes to the text storage. The notification object is the text storage object that processed the edits. This notification doesn’t contain a `userInfo` dictionary.

## See Also

### Notifications

class let willProcessEditingNotification: NSNotification.Name

A notification that posts before a text storage begins processing edits.

