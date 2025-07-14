

- AppKit
- NSPopUpButtonCell
-  titleOfSelectedItem 

Instance Property

# titleOfSelectedItem

The title of the item last selected by the user.

macOS

``` source
@MainActor
var titleOfSelectedItem: String? { get }
```

## Discussion

The value of this property is the title of the selected menu item, or an empty string if no item is selected.

## See Also

### Related Documentation

func selectItem(withTitle: String)

Selects the item with the specified title.

### Title conveniences

func itemTitle(at: Int) -> String

Returns the title of the item at the specified index.

var itemTitles: [String]

An array of `NSString` objects containing the titles of every item in the menu.

