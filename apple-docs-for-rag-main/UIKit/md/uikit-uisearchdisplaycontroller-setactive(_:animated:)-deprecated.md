

- UIKit
- UISearchDisplayController
-  setActive(\_:animated:) Deprecated

Instance Method

# setActive(\_:animated:)

Displays or hides the search interface, optionally with animation.

iOS 3.0–8.0DeprecatediPadOS 3.0–8.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
func setActive(
    _ visible: Bool,
    animated: Bool
)
```

Deprecated

UISearchDisplayController has been replaced with UISearchController

## Parameters 

`visible`  

true to display the search interface if it is not already displayed; false to hide the search interface if it is currently displayed.

`animated`  

true to use animation for a change in visible state, otherwise false.

## Discussion

When the user focus in the search field of a managed search bar, the search display controller automatically displays the search interface. You can use this method to force the search interface to appear.

## See Also

### Displaying the search Interface

var isActive: Bool

The visibility state of the search interface.

Deprecated

