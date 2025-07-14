

- UIKit
- UINavigationItem
-  backButtonDisplayMode 

Instance Property

# backButtonDisplayMode

The display mode of the Back button.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
@MainActor
var backButtonDisplayMode: UINavigationItem.BackButtonDisplayMode { get set }
```

## Discussion

When the `backBarButtonItem` property is `nil`, the navigation item uses this display mode to determine the title of its Back button. The default value of this property is UINavigationItem.BackButtonDisplayMode.default.

## See Also

### Configuring the Back button

var backBarButtonItem: UIBarButtonItem?

The bar button item for adding a Back button to the navigation bar.

var backButtonTitle: String?

The custom title of the Back button.

enum BackButtonDisplayMode

Constants that describe the display modes of the Back button.

var hidesBackButton: Bool

A Boolean value that determines whether the navigation item hides the Back button.

func setHidesBackButton(Bool, animated: Bool)

Hides or shows the Back button, optionally animating the transition.

var backAction: UIAction?

The back action for the navigation bar.

