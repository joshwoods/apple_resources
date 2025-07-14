

- AppKit
- NSApplication
-  searchString(\_:inUserInterfaceItemString:range:found:) 

Instance Method

# searchString(\_:inUserInterfaceItemString:range:found:)

Searches for the string in the user interface.

macOS 10.6+

``` source
@MainActor
func searchString(
    _ searchString: String,
    inUserInterfaceItemString stringToSearch: String,
    range searchRange: NSRange,
    found foundRange: UnsafeMutablePointer?
) -> Bool
```

## Parameters 

`searchString`  

The search string.

`stringToSearch`  

The string to search.

`searchRange`  

The subrange of the `stringToSearch` to restrict the search to.

`foundRange`  

Returns, by-reference, the range of the `searchString` within `stringToSearch`.

## Return Value

true if the searchString is matched, otherwise false.

## Discussion

The search uses the default matching rules for Spotlight for Help.

## See Also

### Providing Help Information

func registerUserInterfaceItemSearchHandler(any NSUserInterfaceItemSearching)

Register an object that provides help data to your app.

func unregisterUserInterfaceItemSearchHandler(any NSUserInterfaceItemSearching)

Unregister an object that provides help data to your app.

func showHelp(Any?)

If your project is properly registered, and the necessary keys have been set in the property list, this method launches Help Viewer and displays the first page of your app’s help book.

func activateContextHelpMode(Any?)

Places the receiver in context-sensitive help mode.

var helpMenu: NSMenu?

The help menu used by the app.

