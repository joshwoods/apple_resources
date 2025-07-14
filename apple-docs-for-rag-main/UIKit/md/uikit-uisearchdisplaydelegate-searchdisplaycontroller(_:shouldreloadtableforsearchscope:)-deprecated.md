

- UIKit
- UISearchDisplayDelegate
-  searchDisplayController(\_:shouldReloadTableForSearchScope:) Deprecated

Instance Method

# searchDisplayController(\_:shouldReloadTableForSearchScope:)

Asks the delegate if the table view should be reloaded for a given scope.

iOS 3.0–8.0DeprecatediPadOS 3.0–8.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
optional func searchDisplayController(
    _ controller: UISearchDisplayController,
    shouldReloadTableForSearchScope searchOption: Int
) -> Bool
```

## Parameters 

`controller`  

The search display controller for which the receiver is the delegate.

`searchOption`  

The index of the selected scope button in the search bar.

## Return Value

true if the display controller should reload the data in its table view, otherwise false.

## Discussion

If you don’t implement this method, then the results table is reloaded as soon as the scope button selection changes.

You might implement this method if you want to perform an asynchronous search: you would initiate the search in this method, then return false, and reload the table when you have results.

## See Also

### Related Documentation

var selectedScopeButtonIndex: Int

The index of the selected scope button.

### Responding to changes in search criteria

func searchDisplayController(UISearchDisplayController, shouldReloadTableForSearch: String?) -> Bool

Asks the delegate if the table view should be reloaded for a given search string.

Deprecated

