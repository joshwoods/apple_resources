

- AppKit
- NSPopUpButtonCell
-  itemTitles 

Instance Property

# itemTitles

An array of `NSString` objects containing the titles of every item in the menu.

macOS

``` source
@MainActor
var itemTitles: [String] { get }
```

## Discussion

The titles appear in the order in which the items appear in the menu. If the menu contains separator items, the array contains an empty string (`@""`) for each separator item.

## See Also

### Title conveniences

func itemTitle(at: Int) -> String

Returns the title of the item at the specified index.

var titleOfSelectedItem: String?

The title of the item last selected by the user.

