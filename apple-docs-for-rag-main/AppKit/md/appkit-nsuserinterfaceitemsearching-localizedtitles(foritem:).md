

- AppKit
- NSUserInterfaceItemSearching
-  localizedTitles(forItem:) 

Instance Method

# localizedTitles(forItem:)

Returns an array of localized strings that will form the help menu item.

macOS

``` source
func localizedTitles(forItem item: Any) -> [String]
```

**Required**

## Parameters 

`item`  

At item in the help menu.

## Return Value

An `NSArray` of `NSStrings` (localized for display in the menu) that will be combined with separators to form the menu item title.

## See Also

### Show Help Menu

func showAllHelpTopics(forSearch: String)

If this method is implemented, a “Show All Help Topics” item will appear in the menu and this method is called when the user selects it.

