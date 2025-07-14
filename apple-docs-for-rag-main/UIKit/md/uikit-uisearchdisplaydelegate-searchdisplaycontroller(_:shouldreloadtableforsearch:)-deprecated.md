

- UIKit
- UISearchDisplayDelegate
-  searchDisplayController(\_:shouldReloadTableForSearch:) Deprecated

Instance Method

# searchDisplayController(\_:shouldReloadTableForSearch:)

Asks the delegate if the table view should be reloaded for a given search string.

iOS 3.0–8.0DeprecatediPadOS 3.0–8.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
optional func searchDisplayController(
    _ controller: UISearchDisplayController,
    shouldReloadTableForSearch searchString: String?
) -> Bool
```

## Parameters 

`controller`  

The search display controller for which the receiver is the delegate.

`searchString`  

The string in the search bar.

## Return Value

true if the display controller should reload the data in its table view, otherwise false.

## Discussion

If you don’t implement this method, then the results table is reloaded as soon as the search string changes.

You might implement this method if you want to perform an asynchronous search. You would initiate the search in this method, then return false. You would reload the table when you have results.

## See Also

### Responding to changes in search criteria

func searchDisplayController(UISearchDisplayController, shouldReloadTableForSearchScope: Int) -> Bool

Asks the delegate if the table view should be reloaded for a given scope.

Deprecated

