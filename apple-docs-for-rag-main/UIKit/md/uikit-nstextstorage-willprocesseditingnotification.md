

- UIKit
- NSTextStorage
-  willProcessEditingNotification 

Type Property

# willProcessEditingNotification

A notification that posts before a text storage begins processing edits.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
class let willProcessEditingNotification: NSNotification.Name
```

## Discussion

The framework posts this notification before a text storage begins processing edits in processEditing(). Observers other than the delegate shouldn’t make further changes to the text storage. The notification object is the text storage object that’s about to process the edits. This notification doesn’t contain a `userInfo` dictionary.

## See Also

### Notifications

class let didProcessEditingNotification: NSNotification.Name

A notification that posts after a text storage finishes processing edits.

