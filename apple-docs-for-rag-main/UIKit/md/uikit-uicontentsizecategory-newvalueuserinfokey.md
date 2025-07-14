

- UIKit
- UIContentSizeCategory
-  newValueUserInfoKey 

Type Property

# newValueUserInfoKey

A key that reflects the new preferred content size.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
nonisolated
static let newValueUserInfoKey: String
```

## Discussion

This key’s value is an NSString object that reflects the new value of the preferredContentSizeCategory property.

## See Also

### Managing the preferred content size

var preferredContentSizeCategory: UIContentSizeCategory

The font sizing option preferred by the user.

struct UIContentSizeCategory

Constants that indicate the preferred size of your content.

protocol UIContentSizeCategoryAdjusting

A collection of methods that give controls an easy way to adopt automatic adjustment to content category changes.

static let didChangeNotification: NSNotification.Name

A notification that posts when the user changes the preferred content size setting.

