

- UIKit
- UIView
-  userInterfaceLayoutDirection(for:relativeTo:) 

Type Method

# userInterfaceLayoutDirection(for:relativeTo:)

Returns the layout direction implied by the specified semantic content attribute, relative to the specified layout direction.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
class func userInterfaceLayoutDirection(
    for semanticContentAttribute: UISemanticContentAttribute,
    relativeTo layoutDirection: UIUserInterfaceLayoutDirection
) -> UIUserInterfaceLayoutDirection
```

## Parameters 

`semanticContentAttribute`  

The semantic content attribute for a view.

`layoutDirection`  

The user interface layout direction (UIUserInterfaceLayoutDirection.leftToRight or UIUserInterfaceLayoutDirection.rightToLeft).

## Return Value

The layout direction implied by the semantic content attribute and relative to the layout direction.

## Discussion

For example, when this method is passed a layout direction of UIUserInterfaceLayoutDirection.rightToLeft and a semantic content attribute of UISemanticContentAttribute.playback, it returns UIUserInterfaceLayoutDirection.leftToRight. Although layout and drawing code can use this method to determine how to arrange elements, it might be easier to query the container view’s effectiveUserInterfaceLayoutDirection property instead.

## See Also

### Adjusting the user interface

var overrideUserInterfaceStyle: UIUserInterfaceStyle

The user interface style adopted by the view and all of its subviews.

var semanticContentAttribute: UISemanticContentAttribute

A semantic description of the view’s contents, used to determine whether the view should be flipped when switching between left-to-right and right-to-left layouts.

var effectiveUserInterfaceLayoutDirection: UIUserInterfaceLayoutDirection

The user interface layout direction appropriate for arranging the immediate content of the view.

class func userInterfaceLayoutDirection(for: UISemanticContentAttribute) -> UIUserInterfaceLayoutDirection

Returns the user interface direction for the given semantic content attribute.

