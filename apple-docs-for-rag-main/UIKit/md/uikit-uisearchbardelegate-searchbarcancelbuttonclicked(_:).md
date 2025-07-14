

- UIKit
- UISearchBarDelegate
-  searchBarCancelButtonClicked(\_:) 

Instance Method

# searchBarCancelButtonClicked(\_:)

Tells the delegate that the cancel button was tapped.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func searchBarCancelButtonClicked(_ searchBar: UISearchBar)
```

## Parameters 

`searchBar`  

The search bar that was tapped.

## Discussion

Typically, you implement this method to dismiss the search bar.

## See Also

### Related Documentation

var showsCancelButton: Bool

A Boolean value indicating whether the cancel button is displayed.

### Responding to clicks in search controls

func searchBarBookmarkButtonClicked(UISearchBar)

Tells the delegate that the bookmark button was tapped.

func searchBarSearchButtonClicked(UISearchBar)

Tells the delegate that the search button was tapped.

func searchBarResultsListButtonClicked(UISearchBar)

Tells the delegate that the search results list button was tapped.

