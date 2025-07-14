

- UIKit
-  UIScrollViewAccessibilityDelegate 

Protocol

# UIScrollViewAccessibilityDelegate

A set of methods you can implement to provide accessibility information for a scroll view.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UIScrollViewAccessibilityDelegate : UIScrollViewDelegate
```

## Topics

### Providing descriptive information

func accessibilityScrollStatus(for: UIScrollView) -> String?

Returns a string describing the content at the current offset in the scroll view.

func accessibilityAttributedScrollStatus(for: UIScrollView) -> NSAttributedString?

Returns an attributed string describing the content at the current offset in the scroll view.

## Relationships

### Inherits From

- NSObjectProtocol
- UIScrollViewDelegate

## See Also

### Elements

class UIAccessibilityElement

An element that should be accessible to users with disabilities, but that isn’t accessible by default.

protocol UIPickerViewAccessibilityDelegate

A set of methods you can implement to provide accessibility information for individual components of a picker view.

