

- UIKit
- UISearchBarDelegate
-  searchBarSearchButtonClicked(\_:) 

Instance Method

# searchBarSearchButtonClicked(\_:)

Tells the delegate that the search button was tapped.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func searchBarSearchButtonClicked(_ searchBar: UISearchBar)
```

## Parameters 

`searchBar`  

The search bar that was tapped.

## Discussion

You should implement this method to begin the search. Use the text property of the search bar to get the text. You can also send becomeFirstResponder() to the search bar to begin editing programmatically.

## See Also

### Responding to clicks in search controls

func searchBarBookmarkButtonClicked(UISearchBar)

Tells the delegate that the bookmark button was tapped.

func searchBarCancelButtonClicked(UISearchBar)

Tells the delegate that the cancel button was tapped.

func searchBarResultsListButtonClicked(UISearchBar)

Tells the delegate that the search results list button was tapped.

