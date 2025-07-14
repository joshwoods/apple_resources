

- AppKit
- NSToolbarItemGroup
-  isSelected(at:) 

Instance Method

# isSelected(at:)

Indicates whether a specified index is currently selected.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+

``` source
@MainActor
func isSelected(at index: Int) -> Bool
```

## Parameters 

`index`  

The index of the subitems in a grouped toolbar item.

## Return Value

A Boolean value indicating whether the specified index is currently selected.

## Discussion

Use this method when you specify the NSToolbarItemGroup.SelectionMode.selectAny selection mode for the grouped toolbar item to determine which subitems are currently selected.

## See Also

### Working with subitems

var subitems: [NSToolbarItem]

The subitems of the grouped toolbar item.

var selectedIndex: Int

The index value for the most recently selected subitem of a grouped toolbar item.

func setSelected(Bool, at: Int)

Sets the selected state of a subitem in a grouped toolbar item.

