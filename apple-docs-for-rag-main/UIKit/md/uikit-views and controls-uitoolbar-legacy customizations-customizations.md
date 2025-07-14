

- UIKit
- Views and controls
- UIToolbar
-  Legacy customizations 

API Collection

# Legacy customizations

Customize appearance information directly on the toolbar object.

## Overview

In iOS 13 and later, customize your toolbar using the standardAppearance and compactAppearance properties. You may continue to use these legacy accessors to customize your toolbar’s appearance directly, but you must update the appearance for different bar configurations yourself.

## Topics

### Setting the bar’s style

var barStyle: UIBarStyle

The toolbar style that specifies its appearance.

enum UIBarStyle

Defines the stylistic appearance of different types of views.

### Configuring bar button items

var tintColor: UIColor!

The tint color to apply to the bar button items.

### Changing the background

var barTintColor: UIColor?

The tint color to apply to the toolbar background.

func backgroundImage(forToolbarPosition: UIBarPosition, barMetrics: UIBarMetrics) -> UIImage?

Returns the image to use for the background in a given position and with given metrics.

func setBackgroundImage(UIImage?, forToolbarPosition: UIBarPosition, barMetrics: UIBarMetrics)

Sets the image to use for the background in a given position and with given metrics.

### Adding a shadow

func shadowImage(forToolbarPosition: UIBarPosition) -> UIImage?

Returns the image to use for the toolbar shadow in a given position.

func setShadowImage(UIImage?, forToolbarPosition: UIBarPosition)

Sets the image to use for the toolbar shadow in a given position.

## See Also

### Customizing appearance

var standardAppearance: UIToolbarAppearance

The appearance settings to use for a standard-height toolbar.

var compactAppearance: UIToolbarAppearance?

The appearance settings to use for a compact-height toolbar.

var scrollEdgeAppearance: UIToolbarAppearance?

The appearance settings for a standard-height toolbar when the edge of scrollable content aligns with the edge of the toolbar.

var compactScrollEdgeAppearance: UIToolbarAppearance?

The appearance settings for a compact-height toolbar when the edge of any scrollable content aligns with the edge of a compact-height toolbar.

var isTranslucent: Bool

A Boolean value that indicates whether the toolbar is translucent.

