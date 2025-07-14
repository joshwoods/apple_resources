

- UIKit
- UINavigationController
-  setNavigationBarHidden(\_:animated:) 

Instance Method

# setNavigationBarHidden(\_:animated:)

Sets whether the navigation bar is hidden.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setNavigationBarHidden(
    _ hidden: Bool,
    animated: Bool
)
```

## Parameters 

`hidden`  

Specify true to hide the navigation bar or false to show it.

`animated`  

Specify true if you want to animate the change in visibility or false if you want the navigation bar to appear immediately.

## Discussion

For animated transitions, the duration of the animation is specified by the value in the hideShowBarDuration constant.

## See Also

### Related Documentation

var isNavigationBarHidden: Bool

A Boolean value that indicates whether the navigation bar is hidden.

### Configuring navigation bars

var navigationBar: UINavigationBar

The navigation bar managed by the navigation controller.

Customizing your app’s navigation bar

Create custom titles, prompts, and buttons in your app’s navigation bar.

