

- UIKit
- UIAccessibilityContentSizeCategoryImageAdjusting
-  adjustsImageSizeForAccessibilityContentSizeCategory 

Instance Property

# adjustsImageSizeForAccessibilityContentSizeCategory

A Boolean value that indicates whether the image size increases to support accessibility content size categories.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var adjustsImageSizeForAccessibilityContentSizeCategory: Bool { get set }
```

**Required**

## Discussion

When the value of this property is true, the current object scales its image to an appropriate accessibility content size category. When the value of this property is false, the current object displays its image at the regular content sizes.

