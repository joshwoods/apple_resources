

- UIKit
- UIView
-  overrideUserInterfaceStyle 

Instance Property

# overrideUserInterfaceStyle

The user interface style adopted by the view and all of its subviews.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var overrideUserInterfaceStyle: UIUserInterfaceStyle { get set }
```

## Mentioned in 

Choosing a Specific Interface Style for Your iOS App

## Discussion

Use this property to force the view to always adopt a light or dark interface style. The default value of this property is UIUserInterfaceStyle.unspecified, which causes the view to inherit the interface style from a parent view or view controller. If you assign a different value, the new style applies to the view and all of the subviews owned by the same view controller. (If the view hierarchy contains the root view of an embedded child view controller, the child view controller and its views do not inherit the interface style.) If the view is a UIWindow object, the new style applies to everything in the window, including the root view controller and all presented content.

## See Also

### Adjusting the user interface

var semanticContentAttribute: UISemanticContentAttribute

A semantic description of the view’s contents, used to determine whether the view should be flipped when switching between left-to-right and right-to-left layouts.

var effectiveUserInterfaceLayoutDirection: UIUserInterfaceLayoutDirection

The user interface layout direction appropriate for arranging the immediate content of the view.

class func userInterfaceLayoutDirection(for: UISemanticContentAttribute) -> UIUserInterfaceLayoutDirection

Returns the user interface direction for the given semantic content attribute.

class func userInterfaceLayoutDirection(for: UISemanticContentAttribute, relativeTo: UIUserInterfaceLayoutDirection) -> UIUserInterfaceLayoutDirection

Returns the layout direction implied by the specified semantic content attribute, relative to the specified layout direction.

