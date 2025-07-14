

- UIKit
- UIView
-  semanticContentAttribute 

Instance Property

# semanticContentAttribute

A semantic description of the view’s contents, used to determine whether the view should be flipped when switching between left-to-right and right-to-left layouts.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var semanticContentAttribute: UISemanticContentAttribute { get set }
```

## Discussion

Some views should not flip when switching between left-to-right and right-to-left layouts. For example, the view is part of the playback controls or represents physical directions (up, down, left, right) that don’t change. Instead of thinking about whether or not a view should change its orientation, select the semantic content attribute that best describes your view.

When creating a view that contains subviews, you can use the userInterfaceLayoutDirection(for:) class method to determine whether the subviews should be flipped, and lay out the views in the appropriate order.

For a list of possible values, see UISemanticContentAttribute.

## See Also

### Adjusting the user interface

var overrideUserInterfaceStyle: UIUserInterfaceStyle

The user interface style adopted by the view and all of its subviews.

var effectiveUserInterfaceLayoutDirection: UIUserInterfaceLayoutDirection

The user interface layout direction appropriate for arranging the immediate content of the view.

class func userInterfaceLayoutDirection(for: UISemanticContentAttribute) -> UIUserInterfaceLayoutDirection

Returns the user interface direction for the given semantic content attribute.

class func userInterfaceLayoutDirection(for: UISemanticContentAttribute, relativeTo: UIUserInterfaceLayoutDirection) -> UIUserInterfaceLayoutDirection

Returns the layout direction implied by the specified semantic content attribute, relative to the specified layout direction.

