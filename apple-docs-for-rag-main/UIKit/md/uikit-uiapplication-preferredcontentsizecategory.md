

- UIKit
- UIApplication
-  preferredContentSizeCategory 

Instance Property

# preferredContentSizeCategory

The font sizing option preferred by the user.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var preferredContentSizeCategory: UIContentSizeCategory { get }
```

## Discussion

Users can request that apps display fonts in a size that is larger or smaller than the normal font size defined by the system. For example, a user with a visual impairment might request a larger default font size to make it easier to read text. Font objects returned by the system automatically scale based on the user’s preference. You can use the value of this property to request a font object of the appropriate size.

When the value of this property changes, the app object sends a didChangeNotification notification so that observers can respond accordingly.

For a list of possible values, see `Content Size Category Constants` and `Accessibility Content Size Category Constants`.

## See Also

### Managing the preferred content size

struct UIContentSizeCategory

Constants that indicate the preferred size of your content.

protocol UIContentSizeCategoryAdjusting

A collection of methods that give controls an easy way to adopt automatic adjustment to content category changes.

static let didChangeNotification: NSNotification.Name

A notification that posts when the user changes the preferred content size setting.

static let newValueUserInfoKey: String

A key that reflects the new preferred content size.

