

- UIKit
- UIView
-  userInterfaceLayoutDirection(for:) 

Type Method

# userInterfaceLayoutDirection(for:)

Returns the user interface direction for the given semantic content attribute.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
class func userInterfaceLayoutDirection(for attribute: UISemanticContentAttribute) -> UIUserInterfaceLayoutDirection
```

## Parameters 

`attribute`  

The semantic content attribute for a view.

## Return Value

The user interface layout direction (left-to-right or right-to-left).

## Discussion

When creating a view that contains subviews, you can use this method to determine whether the subviews should be flipped, and lay out the views in the appropriate order.

## See Also

### Adjusting the user interface

var overrideUserInterfaceStyle: UIUserInterfaceStyle

The user interface style adopted by the view and all of its subviews.

var semanticContentAttribute: UISemanticContentAttribute

A semantic description of the view’s contents, used to determine whether the view should be flipped when switching between left-to-right and right-to-left layouts.

var effectiveUserInterfaceLayoutDirection: UIUserInterfaceLayoutDirection

The user interface layout direction appropriate for arranging the immediate content of the view.

class func userInterfaceLayoutDirection(for: UISemanticContentAttribute, relativeTo: UIUserInterfaceLayoutDirection) -> UIUserInterfaceLayoutDirection

Returns the layout direction implied by the specified semantic content attribute, relative to the specified layout direction.

