

- UIKit
- UINavigationController
-  setToolbarHidden(\_:animated:) 

Instance Method

# setToolbarHidden(\_:animated:)

Changes the visibility of the navigation controller’s built-in toolbar.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func setToolbarHidden(
    _ hidden: Bool,
    animated: Bool
)
```

## Parameters 

`hidden`  

Specify true to hide the toolbar or false to show it.

`animated`  

Specify true if you want the toolbar to be animated on or off the screen.

## Discussion

You can use this method to animate changes to the visibility of the built-in toolbar.

Calling this method with the `animated` parameter set to false is equivalent to setting the value of the isToolbarHidden property directly. The toolbar simply appears or disappears depending on the value in the `hidden` parameter.

## See Also

### Configuring custom toolbars

var toolbar: UIToolbar!

The custom toolbar associated with the navigation controller.

var isToolbarHidden: Bool

A Boolean indicating whether the navigation controller’s built-in toolbar is visible.

class let hideShowBarDuration: CGFloat

A variable that specifies the duration when animating the navigation bar.

