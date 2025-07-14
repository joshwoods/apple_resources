

- UIKit
- UIView
-  safeAreaInsetsDidChange() 

Instance Method

# safeAreaInsetsDidChange()

Called when the safe area of the view changes.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
func safeAreaInsetsDidChange()
```

## See Also

### Getting the safe area

Positioning content relative to the safe area

Position views so that they aren’t obstructed by other content.

var safeAreaInsets: UIEdgeInsets

The insets that you use to determine the safe area for this view.

var safeAreaLayoutGuide: UILayoutGuide

The layout guide representing the portion of your view that is unobscured by bars and other content.

var insetsLayoutMarginsFromSafeArea: Bool

A Boolean value indicating whether the view’s layout margins are updated automatically to reflect the safe area.

