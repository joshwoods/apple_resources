

- UIKit
- UISearchBarDelegate
-  searchBar(\_:selectedScopeButtonIndexDidChange:) 

Instance Method

# searchBar(\_:selectedScopeButtonIndexDidChange:)

Tells the delegate that the scope button selection changed.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func searchBar(
    _ searchBar: UISearchBar,
    selectedScopeButtonIndexDidChange selectedScope: Int
)
```

## Parameters 

`searchBar`  

The search bar that was tapped.

`selectedScope`  

The index of the selected scope button (see selectedScopeButtonIndex).

