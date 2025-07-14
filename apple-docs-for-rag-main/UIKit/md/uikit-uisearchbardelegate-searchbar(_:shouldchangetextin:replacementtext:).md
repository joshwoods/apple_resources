

- UIKit
- UISearchBarDelegate
-  searchBar(\_:shouldChangeTextIn:replacementText:) 

Instance Method

# searchBar(\_:shouldChangeTextIn:replacementText:)

Ask the delegate if text in a specified range should be replaced with given text.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func searchBar(
    _ searchBar: UISearchBar,
    shouldChangeTextIn range: NSRange,
    replacementText text: String
) -> Bool
```

## Parameters 

`searchBar`  

The search bar that is being edited.

`range`  

The range of the text to be changed.

`text`  

The text to replace existing text in `range`.

## Return Value

true if text in `range` should be replaced by `text`, otherwise, false.

## See Also

### Managing the search text

func searchBar(UISearchBar, textDidChange: String)

Tells the delegate that the user changed the search text.

func searchBarShouldBeginEditing(UISearchBar) -> Bool

Asks the delegate if editing should begin in the specified search bar.

func searchBarTextDidBeginEditing(UISearchBar)

Tells the delegate when the user begins editing the search text.

func searchBarShouldEndEditing(UISearchBar) -> Bool

Asks the delegate if editing should stop in the specified search bar.

func searchBarTextDidEndEditing(UISearchBar)

Tells the delegate that the user finished editing the search text.

