

- UIKit
- UIBarButtonItem
-  tintColor 

Instance Property

# tintColor

The tint color to apply to the button item.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var tintColor: UIColor? { get set }
```

## Discussion

In iOS 7 and later, all subclasses of UIView derive their behavior for tintColor from the base class. Although UIBarButtonItem isn’t a view, its tintColor property behaves the same as that of UIView. See the discussion of tintColor in UIView for more information.

## See Also

### Customizing item appearance

var style: UIBarButtonItem.Style

The style of the item.

enum Style

Constants that specify the style of an item.

var isHidden: Bool

A Boolean that determines the visibility of the item.

var isSelected: Bool

A Boolean value that indicates whether the button is in a selected state.

var width: CGFloat

The width of the item.

var possibleTitles: Set&lt;String>?

The set of possible titles to display on the bar button.

