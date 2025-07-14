

- UIKit
-  UITabBarAppearance 

Class

# UITabBarAppearance

An object for customizing the appearance of a tab bar.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class UITabBarAppearance
```

## Overview

After creating a UITabBarAppearance object, use the methods and properties of this class to specify the appearance of items in the tab bar. Use the inherited properties from UIBarAppearance to configure the background and shadow attributes of the tab bar itself.

## Topics

### Configuring stacked item appearances

var stackedLayoutAppearance: UITabBarItemAppearance

The appearance attributes for items with a stacked layout.

var stackedItemPositioning: UITabBar.ItemPositioning

The scheme to use when positioning stacked items within the tab bar.

var stackedItemSpacing: CGFloat

The amount of space to insert between stacked tab bar items.

var stackedItemWidth: CGFloat

The width of stacked items in the tab bar.

### Configuring inline item appearances

var inlineLayoutAppearance: UITabBarItemAppearance

The appearance attributes for items displayed with an inline style.

var compactInlineLayoutAppearance: UITabBarItemAppearance

The appearance attributes for items displayed with an inline style in a compact environment.

### Specifying the selection appearance

var selectionIndicatorTintColor: UIColor?

The tint color to apply to the selection indicator image.

var selectionIndicatorImage: UIImage?

The image to draw for the selected item.

## Relationships

### Inherits From

- UIBarAppearance

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Tab bar appearance

class UITabBarItemAppearance

An object for customizing the appearance of tab bar items.

class UITabBarItemStateAppearance

A data object containing the specific customizations for tab bar items in a particular state.

