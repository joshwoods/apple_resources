

- UIKit
- UITraitCollection
-  toolbarItemPresentationSize 

Instance Property

# toolbarItemPresentationSize

The presentation size of a toolbar item in an AppKit toolbar.

iOS 8.0+iPadOS 8.0+Mac Catalyst 16.0+tvOSvisionOS 1.0+

``` source
var toolbarItemPresentationSize: UINSToolbarItemPresentationSize { get }
```

## Mentioned in 

Building a desktop-class iPad app

## Discussion

NSToolbar supports various display modes that affect the amount of space available for displaying toolbar items. If you use NSUIViewToolbarItem to host a UIView in an NSToolbar when you build your app with Mac Catalyst, that view receives information about its expected size through this trait. Use this trait to make any necessary adjustments to your custom view when the trait collection changes, such as when the toolbar switches to a new display mode.

The default value of this trait is UINSToolbarItemPresentationSize.unspecified when an NSToolbar doesn’t host the view.

## See Also

### Retrieving interface-related traits

var userInterfaceStyle: UIUserInterfaceStyle

The style associated with the user interface.

enum UIUserInterfaceStyle

Constants that indicate the interface style for the app.

var userInterfaceIdiom: UIUserInterfaceIdiom

The user interface idiom of the trait collection.

enum UIUserInterfaceIdiom

Constants that indicate the interface type for the device or an object that has a trait environment, such as a view and view controller.

var userInterfaceLevel: UIUserInterfaceLevel

The elevation level of the interface.

enum UIUserInterfaceLevel

Constants that indicate the visual level for content in the window.

var layoutDirection: UITraitEnvironmentLayoutDirection

The layout direction associated with the current environment.

enum UITraitEnvironmentLayoutDirection

Constants that indicate the layout direction associated with the current environment.

var accessibilityContrast: UIAccessibilityContrast

The accessibility contrast associated with the current environment.

enum UIAccessibilityContrast

Constants that indicate the accessibility contrast setting.

var legibilityWeight: UILegibilityWeight

The font weight to apply to text.

enum UILegibilityWeight

Constants that indicate the weight to apply to text in your interface.

var activeAppearance: UIUserInterfaceActiveAppearance

A property that indicates whether the user interface has an active appearance.

enum UIUserInterfaceActiveAppearance

Constants that indicate whether the user interface has an active appearance.

enum UINSToolbarItemPresentationSize

Constants that specify the presentation size of a toolbar item in an AppKit toolbar.

