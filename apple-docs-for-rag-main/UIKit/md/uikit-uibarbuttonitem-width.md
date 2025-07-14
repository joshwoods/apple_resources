

- UIKit
- UIBarButtonItem
-  width 

Instance Property

# width

The width of the item.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var width: CGFloat { get set }
```

## Discussion

If this property value is positive, the width of the combined image and title are fixed. If the value is `0.0` or negative, the item sets the width of the combined image and title to fit. This property is ignored if the style uses radio mode. The default value is `0.0`.

## See Also

### Customizing item appearance

var style: UIBarButtonItem.Style

The style of the item.

enum Style

Constants that specify the style of an item.

var tintColor: UIColor?

The tint color to apply to the button item.

var isHidden: Bool

A Boolean that determines the visibility of the item.

var isSelected: Bool

A Boolean value that indicates whether the button is in a selected state.

var possibleTitles: Set&lt;String>?

The set of possible titles to display on the bar button.

