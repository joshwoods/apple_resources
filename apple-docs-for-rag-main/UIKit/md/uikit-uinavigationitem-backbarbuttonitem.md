

- UIKit
- UINavigationItem
-  backBarButtonItem 

Instance Property

# backBarButtonItem

The bar button item for adding a Back button to the navigation bar.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var backBarButtonItem: UIBarButtonItem? { get set }
```

## Discussion

When this navigation item is immediately below the top item in the stack, the navigation controller derives the Back button for the navigation bar from this navigation item. If you want to specify a custom title or image for the Back button, you can assign a custom bar button item (with your custom title or image) to this property. When you configure your bar button item, don’t assign a custom view to it; the navigation item ignores custom views in the backBarButtonItem.

When this property is `nil`, the navigation item determines the title of its Back button according to its backButtonDisplayMode. The default value of this property is `nil`.

## See Also

### Related Documentation

var backItem: UINavigationItem?

The navigation item that is immediately below the topmost item on a navigation bar’s stack.

### Configuring the Back button

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

var backAction: UIAction?

The back action for the navigation bar.

