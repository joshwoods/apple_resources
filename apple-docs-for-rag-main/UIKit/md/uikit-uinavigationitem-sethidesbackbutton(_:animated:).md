

- UIKit
- UINavigationItem
-  setHidesBackButton(\_:animated:) 

Instance Method

# setHidesBackButton(\_:animated:)

Hides or shows the Back button, optionally animating the transition.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func setHidesBackButton(
    _ hidesBackButton: Bool,
    animated: Bool
)
```

## Parameters 

`hidesBackButton`  

Specify true if the Back button should be hidden when this navigation item is the top item. Specify false if the Back button should be visible, assuming it hasn’t been replaced by a custom item.

`animated`  

true to animate the transition; otherwise, false.

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

var hidesBackButton: Bool

A Boolean value that determines whether the navigation item hides the Back button.

var backAction: UIAction?

The back action for the navigation bar.

