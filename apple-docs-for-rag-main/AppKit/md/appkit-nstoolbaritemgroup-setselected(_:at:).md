

- AppKit
- NSToolbarItemGroup
-  setSelected(\_:at:) 

Instance Method

# setSelected(\_:at:)

Sets the selected state of a subitem in a grouped toolbar item.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+

``` source
@MainActor
func setSelected(
    _ selected: Bool,
    at index: Int
)
```

## Parameters 

`selected`  

If `true`, indicates whether to select a subitem, `false` otherwise.

`index`  

The index location of the subitem.

## See Also

### Working with subitems

var subitems: [NSToolbarItem]

The subitems of the grouped toolbar item.

var selectedIndex: Int

The index value for the most recently selected subitem of a grouped toolbar item.

func isSelected(at: Int) -> Bool

Indicates whether a specified index is currently selected.

