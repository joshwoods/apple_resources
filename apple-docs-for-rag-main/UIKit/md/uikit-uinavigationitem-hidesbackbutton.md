

- UIKit
- UINavigationItem
-  hidesBackButton 

Instance Property

# hidesBackButton

A Boolean value that determines whether the navigation item hides the Back button.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var hidesBackButton: Bool { get set }
```

## Discussion

When set to true, the Back button is hidden when this navigation item is the top item. This is true regardless of the value in the leftItemsSupplementBackButton property. When set to false, the Back button is shown if it’s still present. (It can be replaced by values in either the leftBarButtonItem or leftBarButtonItems properties.) The default value is false.

## See Also

### Related Documentation

var backItem: UINavigationItem?

The navigation item that is immediately below the topmost item on a navigation bar’s stack.

### Configuring the Back button

var backBarButtonItem: UIBarButtonItem?

The bar button item for adding a Back button to the navigation bar.

var backButtonTitle: String?

The custom title of the Back button.

var backButtonDisplayMode: UINavigationItem.BackButtonDisplayMode

The display mode of the Back button.

enum BackButtonDisplayMode

Constants that describe the display modes of the Back button.

func setHidesBackButton(Bool, animated: Bool)

Hides or shows the Back button, optionally animating the transition.

var backAction: UIAction?

The back action for the navigation bar.

