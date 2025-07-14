

- AppKit
- NSUserInterfaceItemSearching
-  showAllHelpTopics(forSearch:) 

Instance Method

# showAllHelpTopics(forSearch:)

If this method is implemented, a “Show All Help Topics” item will appear in the menu and this method is called when the user selects it.

macOS

``` source
optional func showAllHelpTopics(forSearch searchString: String)
```

## Parameters 

`searchString`  

The search string.

## Discussion

The application should show all its results for this search, which does not include results for menu items. The string for “Show All Help Topics” is system defined and localized and cannot be changed by the user.

## See Also

### Show Help Menu

func localizedTitles(forItem: Any) -> [String]

Returns an array of localized strings that will form the help menu item.

**Required**

