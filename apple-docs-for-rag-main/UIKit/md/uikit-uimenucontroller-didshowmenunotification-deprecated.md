

- UIKit
- UIMenuController
-  didShowMenuNotification Deprecated

Type Property

# didShowMenuNotification

Posted by the menu controller just after it shows the menu.

iOS 3.0–16.0DeprecatediPadOS 3.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
nonisolated
class let didShowMenuNotification: NSNotification.Name
```

Deprecated

Use UIEditMenuInteraction instead.

## Discussion

There is no `userInfo` dictionary.

## See Also

### Notifications

class let willShowMenuNotification: NSNotification.Name

Posted by the menu controller just before it shows the menu.

Deprecated

class let willHideMenuNotification: NSNotification.Name

Posted by the menu controller just before it hides the menu.

Deprecated

class let didHideMenuNotification: NSNotification.Name

Posted by the menu controller just after it hides the menu.

Deprecated

class let menuFrameDidChangeNotification: NSNotification.Name

Posted when the frame of a visible menu changes.

Deprecated

