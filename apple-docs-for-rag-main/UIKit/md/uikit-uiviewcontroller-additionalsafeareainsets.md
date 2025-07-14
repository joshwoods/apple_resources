

- UIKit
- UIViewController
-  additionalSafeAreaInsets 

Instance Property

# additionalSafeAreaInsets

Custom insets that you specify to modify the view controller’s safe area.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var additionalSafeAreaInsets: UIEdgeInsets { get set }
```

## Mentioned in 

Positioning content relative to the safe area

Creating a custom container view controller

## Discussion

Use this property to adjust the safe area insets of this view controller’s views by the specified amount. The safe area defines the portion of your view controller’s visible area that is guaranteed to be unobscured by the system status bar or by an ancestor-provided view such as the navigation bar.

You might use this property to extend the safe area to include custom content in your interface. For example, a drawing app might use this property to avoid displaying content underneath tool palettes.

## See Also

### Extending the view’s safe area

Positioning content relative to the safe area

Position views so that they aren’t obstructed by other content.

func viewSafeAreaInsetsDidChange()

Called to notify the view controller that the safe area insets of its root view changed.

