

- AppKit
- NSToolbarItemGroup
-  selectedIndex 

Instance Property

# selectedIndex

The index value for the most recently selected subitem of a grouped toolbar item.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+

``` source
@MainActor
var selectedIndex: Int { get set }
```

## Discussion

When using the NSToolbarItemGroup.SelectionMode.selectAny or NSToolbarItemGroup.SelectionMode.momentary selection mode, don’t assume that this value represents the selected subitem. This method returns the index of the most recently selected subitem.

To determine if a specific subitem of a grouped toolbar item is selected, use the isSelected(at:) method.

## See Also

### Working with subitems

var subitems: [NSToolbarItem]

The subitems of the grouped toolbar item.

func isSelected(at: Int) -> Bool

Indicates whether a specified index is currently selected.

func setSelected(Bool, at: Int)

Sets the selected state of a subitem in a grouped toolbar item.

