

- UIKit
- UITraitCollection
-  accessibilityContrast 

Instance Property

# accessibilityContrast

The accessibility contrast associated with the current environment.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
var accessibilityContrast: UIAccessibilityContrast { get }
```

## Discussion

Use this trait to determine whether the user requested a high contrast between foreground and background content. The user sets the contrast level in the Accessibility area in Settings.

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

var toolbarItemPresentationSize: UINSToolbarItemPresentationSize

The presentation size of a toolbar item in an AppKit toolbar.

enum UINSToolbarItemPresentationSize

Constants that specify the presentation size of a toolbar item in an AppKit toolbar.

