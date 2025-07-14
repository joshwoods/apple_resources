

- UIKit
- UISearchBarDelegate
-  searchBar(\_:textDidChange:) 

Instance Method

# searchBar(\_:textDidChange:)

Tells the delegate that the user changed the search text.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func searchBar(
    _ searchBar: UISearchBar,
    textDidChange searchText: String
)
```

## Parameters 

`searchBar`  

The search bar that is being edited.

`searchText`  

The current text in the search text field.

## Discussion

This method is also invoked when text is cleared from the search text field.

## See Also

### Managing the search text

func searchBar(UISearchBar, shouldChangeTextIn: NSRange, replacementText: String) -> Bool

Ask the delegate if text in a specified range should be replaced with given text.

func searchBarShouldBeginEditing(UISearchBar) -> Bool

Asks the delegate if editing should begin in the specified search bar.

func searchBarTextDidBeginEditing(UISearchBar)

Tells the delegate when the user begins editing the search text.

func searchBarShouldEndEditing(UISearchBar) -> Bool

Asks the delegate if editing should stop in the specified search bar.

func searchBarTextDidEndEditing(UISearchBar)

Tells the delegate that the user finished editing the search text.

