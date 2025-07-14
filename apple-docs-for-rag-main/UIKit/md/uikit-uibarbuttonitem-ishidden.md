

- UIKit
- UIBarButtonItem
-  isHidden 

Instance Property

# isHidden

A Boolean that determines the visibility of the item.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var isHidden: Bool { get set }
```

## Discussion

Set this property to true to hide the item, or false to display the item.

## See Also

### Customizing item appearance

var style: UIBarButtonItem.Style

The style of the item.

enum Style

Constants that specify the style of an item.

var tintColor: UIColor?

The tint color to apply to the button item.

var isSelected: Bool

A Boolean value that indicates whether the button is in a selected state.

var width: CGFloat

The width of the item.

var possibleTitles: Set&lt;String>?

The set of possible titles to display on the bar button.

