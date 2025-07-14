

- UIKit
- UISearchDisplayController
-  init(searchBar:contentsController:) Deprecated

Initializer

# init(searchBar:contentsController:)

Returns a display controller initialized with the given search bar and contents controller.

iOS 3.0–8.0DeprecatediPadOS 3.0–8.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
init(
    searchBar: UISearchBar,
    contentsController viewController: UIViewController
)
```

## Parameters 

`searchBar`  

A search bar.

The search bar must not currently be associated with another search display controller.

`viewController`  

The view controller that manages display of the original contents that are to be searched.

The view controller must not currently be associated with another search display controller.

## Return Value

A search display controller initialized with the given search bar and contents controller.

