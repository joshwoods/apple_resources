

- UIKit
- UISearchBarDelegate
-  searchBarBookmarkButtonClicked(\_:) 

Instance Method

# searchBarBookmarkButtonClicked(\_:)

Tells the delegate that the bookmark button was tapped.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func searchBarBookmarkButtonClicked(_ searchBar: UISearchBar)
```

## Parameters 

`searchBar`  

The search bar that was tapped.

## Discussion

There is no automatic bookmark support provided by the search bar. It’s the application’s responsibility to implement this method to perform some action if the bookmark button is tapped by the user.

## See Also

### Related Documentation

var showsBookmarkButton: Bool

A Boolean value indicating whether the bookmark button is displayed.

### Responding to clicks in search controls

func searchBarCancelButtonClicked(UISearchBar)

Tells the delegate that the cancel button was tapped.

func searchBarSearchButtonClicked(UISearchBar)

Tells the delegate that the search button was tapped.

func searchBarResultsListButtonClicked(UISearchBar)

Tells the delegate that the search results list button was tapped.

