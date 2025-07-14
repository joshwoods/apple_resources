

- SwiftUI
-  ContentSizeCategory Deprecated

Enumeration

# ContentSizeCategory

The sizes that you can specify for content.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 6.0–11.4Deprecated

``` source
enum ContentSizeCategory
```

Deprecated

Use DynamicTypeSize instead.

## Topics

### Content size categories

case accessibilityExtraExtraExtraLarge

case accessibilityExtraExtraLarge

case accessibilityExtraLarge

case accessibilityLarge

case accessibilityMedium

case extraExtraExtraLarge

case extraExtraLarge

case extraLarge

case extraSmall

case large

case medium

case small

### Creating a size category

init?(UIContentSizeCategory)

Create a size category from its UIContentSizeCategory equivalent.

### Comparing content size categories

var isAccessibilityCategory: Bool

A Boolean value indicating whether the content size category is one that is associated with accessibility.

### Operators

static func &lt; (ContentSizeCategory, ContentSizeCategory) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than that of the second argument.

static func > (ContentSizeCategory, ContentSizeCategory) -> Bool

Returns a Boolean value indicating whether the value of the first argument is greater than that of the second argument.

static func &lt;= (ContentSizeCategory, ContentSizeCategory) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than or equal to that of the second argument.

static func >= (ContentSizeCategory, ContentSizeCategory) -> Bool

Returns a Boolean value indicating whether the value of the first argument is greater than or equal to that of the second argument.

## Relationships

### Conforms To

- CaseIterable
- Equatable
- Hashable

