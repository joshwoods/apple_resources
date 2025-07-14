

- UIKit
- View controllers
- UITabBar
-  Legacy customizations 

API Collection

# Legacy customizations

Customize appearance information directly on the tab bar object.

## Overview

In iOS 13 and later, customize your tab bar using the standardAppearance property. You may also continue to use these legacy accessors to customize your tab bar’s appearance directly.

## Topics

### Setting the bar’s style

var barStyle: UIBarStyle

The tab bar style that specifies its appearance.

enum UIBarStyle

Defines the stylistic appearance of different types of views.

### Configuring tab bar items

var tintColor: UIColor!

The tint color to apply to the tab bar items.

### Customizing item spacing

var itemPositioning: UITabBar.ItemPositioning

The positioning scheme for the tab bar items in the tab bar.

enum ItemPositioning

Constants that specify tab bar item positioning.

var itemSpacing: CGFloat

The amount of space (in points) to use between tab bar items.

var itemWidth: CGFloat

The width (in points) of tab bar items.

### Configuring selection appearance

var unselectedItemTintColor: UIColor?

The tint color to apply to unselected tabs.

var selectionIndicatorImage: UIImage?

The image to use for the selection indicator.

var selectedImageTintColor: UIColor?

The tint color applied to the selected tab bar item.

Deprecated

### Changing the background

var barTintColor: UIColor?

The tint color to apply to the tab bar background.

var backgroundImage: UIImage?

The custom background image for the tab bar.

### Adding a shadow

var shadowImage: UIImage?

The shadow image to use for the tab bar.

## See Also

### Customizing tab bar appearance

var standardAppearance: UITabBarAppearance

The appearance settings for a standard-height tab bar.

var scrollEdgeAppearance: UITabBarAppearance?

The appearance settings for the tab bar when the edge of scrollable content aligns with the edge of the tab bar.

var leadingAccessoryView: UIView

The view at the leading edge of a tab bar on tvOS.

var trailingAccessoryView: UIView

The view at the trailing edge of a tab bar on tvOS.

var isTranslucent: Bool

A Boolean value that indicates whether the tab bar is translucent.

