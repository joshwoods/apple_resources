

- UIKit
- UIContentSizeCategory
-  isAccessibilityCategory 

Instance Property

# isAccessibilityCategory

A Boolean value that indicates whether the content size category is associated with accessibility.

iOS 11.0+iPadOS 11.0+Mac CatalysttvOS 11.0+visionOS

``` source
var isAccessibilityCategory: Bool { get }
```

## Discussion

This property is true for accessibilityMedium, accessibilityLarge, accessibilityExtraLarge, accessibilityExtraExtraLarge, and accessibilityExtraExtraExtraLarge. It is false for other values.

## See Also

### Accessibility sizes

static let accessibilityMedium: UIContentSizeCategory

A medium font size that reflects the current accessibility settings.

static let accessibilityLarge: UIContentSizeCategory

A large font size that reflects the current accessibility settings.

static let accessibilityExtraLarge: UIContentSizeCategory

An extra-large font size that reflects the current accessibility settings.

static let accessibilityExtraExtraLarge: UIContentSizeCategory

A font that is larger than the extra-large font but not the largest available, reflecting the current accessibility settings.

static let accessibilityExtraExtraExtraLarge: UIContentSizeCategory

The largest font size that reflects the current accessibility settings.

