

- UIKit
- UIContentSizeCategoryAdjusting
-  adjustsFontForContentSizeCategory 

Instance Property

# adjustsFontForContentSizeCategory

A Boolean that indicates whether the object automatically updates its font when the device’s content size category changes.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
var adjustsFontForContentSizeCategory: Bool { get set }
```

**Required**

## Mentioned in 

Scaling Fonts Automatically

## Discussion

Set the value of this property to true to allow the element to update its font when the size category changes. Set the value to false to ignore the size category changes.

For this property to take effect, the element’s font must be vended one of the following ways:

- It must be vended using the preferredFont(forTextStyle:) or preferredFont(forTextStyle:compatibleWith:) method with a valid text style.

- It must be vended using one of the scaling methods from UIFontMetrics.

Because fonts are immutable, any element that adjusts for an updated content size category doesn’t modify the font itself. Instead, the element replaces the assigned font with a new instance based on the original settings.

If you set this property to true, the element adjusts for a new content size category on a didChangeNotification.

