

- UIKit
- UISearchBar
-  setShowsCancelButton(\_:animated:) 

Instance Method

# setShowsCancelButton(\_:animated:)

Sets the display state of the cancel button optionally with animation.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func setShowsCancelButton(
    _ showsCancelButton: Bool,
    animated: Bool
)
```

## Parameters 

`showsCancelButton`  

true to display the cancel button, otherwise false.

`animated`  

true to use animation to change the display state of the cancel button, otherwise false.

## Discussion

Cancel buttons are not displayed for apps running on iPad, even when you specify true for the `showsCancelButton` parameter

## See Also

### Configuring the search interface

var showsBookmarkButton: Bool

A Boolean value indicating whether the bookmark button is displayed.

var showsCancelButton: Bool

A Boolean value indicating whether the cancel button is displayed.

var showsSearchResultsButton: Bool

A Boolean value indicating whether the search results button is displayed.

var isSearchResultsButtonSelected: Bool

A Boolean value indicating whether the search results button is selected.

