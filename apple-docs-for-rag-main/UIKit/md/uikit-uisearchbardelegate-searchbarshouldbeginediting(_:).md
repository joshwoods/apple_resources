

- UIKit
- UISearchBarDelegate
-  searchBarShouldBeginEditing(\_:) 

Instance Method

# searchBarShouldBeginEditing(\_:)

Asks the delegate if editing should begin in the specified search bar.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func searchBarShouldBeginEditing(_ searchBar: UISearchBar) -> Bool
```

## Parameters 

`searchBar`  

The search bar that is being edited.

## Return Value

true if an editing session should be initiated, otherwise, false.

## See Also

### Managing the search text

func searchBar(UISearchBar, textDidChange: String)

Tells the delegate that the user changed the search text.

func searchBar(UISearchBar, shouldChangeTextIn: NSRange, replacementText: String) -> Bool

Ask the delegate if text in a specified range should be replaced with given text.

func searchBarTextDidBeginEditing(UISearchBar)

Tells the delegate when the user begins editing the search text.

func searchBarShouldEndEditing(UISearchBar) -> Bool

Asks the delegate if editing should stop in the specified search bar.

func searchBarTextDidEndEditing(UISearchBar)

Tells the delegate that the user finished editing the search text.

