

- UIKit
-  UIContentSizeCategory 

Structure

# UIContentSizeCategory

Constants that indicate the preferred size of your content.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
struct UIContentSizeCategory
```

## Topics

### Font sizes

static let unspecified: UIContentSizeCategory

An unspecified font size.

static let extraSmall: UIContentSizeCategory

An extra-small font.

static let small: UIContentSizeCategory

A small font.

static let medium: UIContentSizeCategory

A medium-sized font.

static let large: UIContentSizeCategory

A large font.

static let extraLarge: UIContentSizeCategory

An extra-large font.

static let extraExtraLarge: UIContentSizeCategory

A font that is larger than the extra-large font but smaller than the largest font size available.

static let extraExtraExtraLarge: UIContentSizeCategory

The largest font size.

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

var isAccessibilityCategory: Bool

A Boolean value that indicates whether the content size category is associated with accessibility.

### Font size change notifications

static let didChangeNotification: NSNotification.Name

A notification that posts when the user changes the preferred content size setting.

static let newValueUserInfoKey: String

A key that reflects the new preferred content size.

### Font size category creation

init(rawValue: String)

Creates a new instance with the specified raw value.

init(ContentSizeCategory?)

Creates a content size category from the specified SwiftUI content size category.

init(DynamicTypeSize?)

Creates a content size category from the specified SwiftUI Dynamic Type size.

## Relationships

### Conforms To

- Comparable
- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing the preferred content size

var preferredContentSizeCategory: UIContentSizeCategory

The font sizing option preferred by the user.

protocol UIContentSizeCategoryAdjusting

A collection of methods that give controls an easy way to adopt automatic adjustment to content category changes.

static let didChangeNotification: NSNotification.Name

A notification that posts when the user changes the preferred content size setting.

static let newValueUserInfoKey: String

A key that reflects the new preferred content size.

