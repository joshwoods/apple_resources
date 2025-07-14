

- UIKit
- UISearchDisplayController
-  isActive Deprecated

Instance Property

# isActive

The visibility state of the search interface.

iOS 3.0–8.0DeprecatediPadOS 3.0–8.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var isActive: Bool { get set }
```

## Discussion

The default value is false.

If you set this value directly, any change is performed without animation. Use setActive(_:animated:) if a change in state should be animated.

When the user focus in the search field of a managed search bar, the search display controller automatically displays the search interface. You can use this property to force the search interface to appear.

## See Also

### Displaying the search Interface

func setActive(Bool, animated: Bool)

Displays or hides the search interface, optionally with animation.

Deprecated

