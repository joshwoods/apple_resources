

- UIKit
- UIView
-  insetsLayoutMarginsFromSafeArea 

Instance Property

# insetsLayoutMarginsFromSafeArea

A Boolean value indicating whether the view’s layout margins are updated automatically to reflect the safe area.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var insetsLayoutMarginsFromSafeArea: Bool { get set }
```

## Mentioned in 

Positioning content within layout margins

## Discussion

When the value of this property is true, any margins that are outside the safe area are automatically modified to fall within the safe area boundary. The default value of this property is true. Changing the value to false allows your margins to remain at their original locations, even when they are outside the safe area.

## See Also

### Getting the safe area

Positioning content relative to the safe area

Position views so that they aren’t obstructed by other content.

var safeAreaInsets: UIEdgeInsets

The insets that you use to determine the safe area for this view.

var safeAreaLayoutGuide: UILayoutGuide

The layout guide representing the portion of your view that is unobscured by bars and other content.

func safeAreaInsetsDidChange()

Called when the safe area of the view changes.

