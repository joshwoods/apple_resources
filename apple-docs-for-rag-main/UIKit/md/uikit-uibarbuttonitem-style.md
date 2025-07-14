

- UIKit
- UIBarButtonItem
-  style 

Instance Property

# style

The style of the item.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var style: UIBarButtonItem.Style { get set }
```

## Discussion

One of the constants defined in UIBarButtonItem.Style. The default value is UIBarButtonItem.Style.plain.

## See Also

### Customizing item appearance

enum Style

Constants that specify the style of an item.

var tintColor: UIColor?

The tint color to apply to the button item.

var isHidden: Bool

A Boolean that determines the visibility of the item.

var isSelected: Bool

A Boolean value that indicates whether the button is in a selected state.

var width: CGFloat

The width of the item.

var possibleTitles: Set&lt;String>?

The set of possible titles to display on the bar button.

