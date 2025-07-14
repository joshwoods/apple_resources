

- UIKit
- UITraitCollection
-  preferredContentSizeCategory 

Instance Property

# preferredContentSizeCategory

The font sizing option preferred by the user.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
var preferredContentSizeCategory: UIContentSizeCategory { get }
```

## Discussion

With Dynamic Type, users can ask that apps display text using fonts that are larger or smaller than the normal font size defined by the system. For example, a user with a visual impairment might request a larger default font size to make it easier to read text. Use the value of this property to request a UIFont object that matches the user’s requested size.

## See Also

### Retrieving content size category information

struct UIContentSizeCategory

Constants that indicate the preferred size of your content.

