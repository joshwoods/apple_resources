

- UIKit
-  UIContentSizeCategoryAdjusting 

Protocol

# UIContentSizeCategoryAdjusting

A collection of methods that give controls an easy way to adopt automatic adjustment to content category changes.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
protocol UIContentSizeCategoryAdjusting : NSObjectProtocol
```

## Topics

### Adjusting the size of fonts

var adjustsFontForContentSizeCategory: Bool

A Boolean that indicates whether the object automatically updates its font when the device’s content size category changes.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- UILabel
- UISearchTextField
- UITextField
- UITextView

## See Also

### Managing the preferred content size

var preferredContentSizeCategory: UIContentSizeCategory

The font sizing option preferred by the user.

struct UIContentSizeCategory

Constants that indicate the preferred size of your content.

static let didChangeNotification: NSNotification.Name

A notification that posts when the user changes the preferred content size setting.

static let newValueUserInfoKey: String

A key that reflects the new preferred content size.

