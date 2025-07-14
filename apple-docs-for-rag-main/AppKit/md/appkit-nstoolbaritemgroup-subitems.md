

- AppKit
- NSToolbarItemGroup
-  subitems 

Instance Property

# subitems

The subitems of the grouped toolbar item.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.5+

``` source
@MainActor
var subitems: [NSToolbarItem] { get set }
```

## Discussion

By default, an NSToolbarItemGroup instance has an empty array of subitems.

## See Also

### Related Documentation

Toolbar Programming Topics for Cocoa

### Working with subitems

var selectedIndex: Int

The index value for the most recently selected subitem of a grouped toolbar item.

func isSelected(at: Int) -> Bool

Indicates whether a specified index is currently selected.

func setSelected(Bool, at: Int)

Sets the selected state of a subitem in a grouped toolbar item.

