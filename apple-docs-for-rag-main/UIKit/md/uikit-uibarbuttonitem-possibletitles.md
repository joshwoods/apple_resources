

- UIKit
- UIBarButtonItem
-  possibleTitles 

Instance Property

# possibleTitles

The set of possible titles to display on the bar button.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var possibleTitles: Set? { get set }
```

## Discussion

Use this property to provide a hint to the system on how to correctly size the bar button item to be wide enough to accommodate your widest title. Set the value of this property to an NSSet object containing all the titles you intend as possible titles for the bar button item. Use the actual text strings you intend to display.

This property applies to bar button items placed on navigation bars or toolbars.

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

var width: CGFloat

The width of the item.

