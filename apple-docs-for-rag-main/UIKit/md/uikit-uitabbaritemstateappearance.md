

- UIKit
-  UITabBarItemStateAppearance 

Class

# UITabBarItemStateAppearance

A data object containing the specific customizations for tab bar items in a particular state.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class UITabBarItemStateAppearance
```

## Overview

Use a UITabBarItemStateAppearance object to customize the appearance of your tab bar items and the badges they display. Don’t create UITabBarItemStateAppearance objects yourself. Instead, create a UITabBarItemAppearance object and use its properties to fetch the appearance attributes for tab bar items in a particular state. For example, to set the attributes for items in the normal state, configure the object in the normal property.

## Topics

### Configuring the item’s title

var titleTextAttributes: [NSAttributedString.Key : Any]

String attributes to apply to the text of the tab bar item’s title.

var titlePositionAdjustment: UIOffset

The additional amount by which to offset the title horizontally and vertically.

### Tinting the item’s icon

var iconColor: UIColor?

The color of item icons.

### Configuring the badge appearance

var badgeTextAttributes: [NSAttributedString.Key : Any]

String attributes to apply to the text of the item’s badge.

var badgeBackgroundColor: UIColor?

The background color of the badge.

var badgeTitlePositionAdjustment: UIOffset

The additional amount by which to offset the badge’s title horizontally and vertically.

var badgePositionAdjustment: UIOffset

The additional amount by which to offset the badge horizontally and vertically.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Tab bar appearance

class UITabBarAppearance

An object for customizing the appearance of a tab bar.

class UITabBarItemAppearance

An object for customizing the appearance of tab bar items.

