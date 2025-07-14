

- UIKit
- UISearchBarDelegate
-  searchBarShouldEndEditing(\_:) 

Instance Method

# searchBarShouldEndEditing(\_:)

Asks the delegate if editing should stop in the specified search bar.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func searchBarShouldEndEditing(_ searchBar: UISearchBar) -> Bool
```

## Parameters 

`searchBar`  

The search bar that is being edited.

## Return Value

true if editing should stop, otherwise false.

## See Also

### Managing the search text

func searchBar(UISearchBar, textDidChange: String)

Tells the delegate that the user changed the search text.

func searchBar(UISearchBar, shouldChangeTextIn: NSRange, replacementText: String) -> Bool

Ask the delegate if text in a specified range should be replaced with given text.

func searchBarShouldBeginEditing(UISearchBar) -> Bool

Asks the delegate if editing should begin in the specified search bar.

func searchBarTextDidBeginEditing(UISearchBar)

Tells the delegate when the user begins editing the search text.

func searchBarTextDidEndEditing(UISearchBar)

Tells the delegate that the user finished editing the search text.

