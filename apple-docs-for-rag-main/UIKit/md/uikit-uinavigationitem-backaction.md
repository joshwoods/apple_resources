

- UIKit
- UINavigationItem
-  backAction 

Instance Property

# backAction

The back action for the navigation bar.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@NSCopying @MainActor
var backAction: UIAction? { get set }
```

## Discussion

If a back button already appears in the navigation bar, setting this property replaces its action without modifying its appearance. Otherwise, setting this property generates a back button with the image or title from the action you specify, unless you use the UINavigationItem.ItemStyle.editor navigation style.

## See Also

### Configuring the Back button

var backBarButtonItem: UIBarButtonItem?

The bar button item for adding a Back button to the navigation bar.

var backButtonTitle: String?

The custom title of the Back button.

var backButtonDisplayMode: UINavigationItem.BackButtonDisplayMode

The display mode of the Back button.

enum BackButtonDisplayMode

Constants that describe the display modes of the Back button.

var hidesBackButton: Bool

A Boolean value that determines whether the navigation item hides the Back button.

func setHidesBackButton(Bool, animated: Bool)

Hides or shows the Back button, optionally animating the transition.

