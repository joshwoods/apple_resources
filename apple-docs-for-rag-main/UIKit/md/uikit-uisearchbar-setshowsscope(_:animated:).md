

- UIKit
- UISearchBar
-  setShowsScope(\_:animated:) 

Instance Method

# setShowsScope(\_:animated:)

Specifies whether the scope bar is displayed, optionally using an animation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
func setShowsScope(
    _ show: Bool,
    animated animate: Bool
)
```

## Parameters 

`show`  

A Boolean value that indicates whether the scope bar is shown.

`animate`  

A Boolean value that indicates whether the scope bar animates when it appears and disappears.

## Discussion

If the search bar is owned by a UISearchController, then calling this method implicitly sets the search controller’s automaticallyShowsScopeBar property to false.

## See Also

### Configuring scope bar buttons

var scopeButtonTitles: [String]?

An array of strings indicating the titles of the scope buttons.

var selectedScopeButtonIndex: Int

The index of the selected scope button.

var showsScopeBar: Bool

Specifies whether the scope bar is displayed.

