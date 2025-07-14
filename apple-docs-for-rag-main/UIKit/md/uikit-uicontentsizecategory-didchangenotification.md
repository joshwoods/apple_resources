

- UIKit
- UIContentSizeCategory
-  didChangeNotification 

Type Property

# didChangeNotification

A notification that posts when the user changes the preferred content size setting.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
nonisolated
static let didChangeNotification: NSNotification.Name
```

## Mentioned in 

Scaling Fonts Automatically

## Discussion

This notification is sent when the value in the preferredContentSizeCategory property changes. The `userInfo` dictionary of the notification contains the newValueUserInfoKey key, which reflects the new setting.

## See Also

### Managing the preferred content size

var preferredContentSizeCategory: UIContentSizeCategory

The font sizing option preferred by the user.

struct UIContentSizeCategory

Constants that indicate the preferred size of your content.

protocol UIContentSizeCategoryAdjusting

A collection of methods that give controls an easy way to adopt automatic adjustment to content category changes.

static let newValueUserInfoKey: String

A key that reflects the new preferred content size.

