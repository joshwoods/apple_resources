

- UIKit
- View controllers
- UINavigationBar
-  Legacy customizations 

API Collection

# Legacy customizations

Customize appearance information directly on the navigation bar object.

## Overview

In iOS 13 and later, customize your navigation bar using the standardAppearance, compactAppearance, and scrollEdgeAppearance properties. You may continue to use these legacy accessors to customize your navigation bar’s appearance directly, but you must update the appearance for different bar configurations yourself.

## Topics

### Configuring the navigation bar

Customizing your app’s navigation bar

Create custom titles, prompts, and buttons in your app’s navigation bar.

### Setting the bar’s style

var barStyle: UIBarStyle

The navigation bar style that specifies its appearance.

enum UIBarStyle

Defines the stylistic appearance of different types of views.

### Configuring the title

var titleTextAttributes: [NSAttributedString.Key : Any]?

Display attributes for the bar’s title text.

var largeTitleTextAttributes: [NSAttributedString.Key : Any]?

Display attributes for the bar’s large title text.

func titleVerticalPositionAdjustment(for: UIBarMetrics) -> CGFloat

Returns the title’s vertical position adjustment for given bar metrics.

func setTitleVerticalPositionAdjustment(CGFloat, for: UIBarMetrics)

Sets the title’s vertical position adjustment for given bar metrics.

### Configuring bar button items

var tintColor: UIColor!

The tint color to apply to the navigation items and bar button items.

### Configuring the Back button

var backIndicatorImage: UIImage?

The image shown beside the Back button.

var backIndicatorTransitionMaskImage: UIImage?

The image used as a mask for content during push and pop transitions.

### Changing the background

var barTintColor: UIColor?

The tint color to apply to the navigation bar background.

func backgroundImage(for: UIBarMetrics) -> UIImage?

Returns the background image for given bar metrics.

func setBackgroundImage(UIImage?, for: UIBarMetrics)

Sets the background image for given bar metrics.

func backgroundImage(for: UIBarPosition, barMetrics: UIBarMetrics) -> UIImage?

Returns the background image to use for a given bar position and set of metrics.

func setBackgroundImage(UIImage?, for: UIBarPosition, barMetrics: UIBarMetrics)

Sets the background image to use for a given bar position and set of metrics.

### Adding a shadow

var shadowImage: UIImage?

The shadow image to be used for the navigation bar.

## See Also

### Customizing the bar’s appearance

var prefersLargeTitles: Bool

A Boolean value that indicates whether the title displays in a large format.

var standardAppearance: UINavigationBarAppearance

The appearance settings for a standard-height navigation bar.

var compactAppearance: UINavigationBarAppearance?

The appearance settings for a compact-height navigation bar.

var scrollEdgeAppearance: UINavigationBarAppearance?

The appearance settings for the navigation bar when the edge of scrollable content aligns with the edge of the navigation bar.

var compactScrollEdgeAppearance: UINavigationBarAppearance?

The appearance settings for a compact-height navigation bar when the edge of scrollable content aligns with the edge of the navigation bar.

var isTranslucent: Bool

A Boolean value that indicates whether the navigation bar is translucent.

