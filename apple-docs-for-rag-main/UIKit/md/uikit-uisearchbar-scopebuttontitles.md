

- UIKit
- UISearchBar
-  scopeButtonTitles 

Instance Property

# scopeButtonTitles

An array of strings indicating the titles of the scope buttons.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var scopeButtonTitles: [String]? { get set }
```

## Discussion

The order of the strings in the array indicates the order that the corresponding buttons will be displayed, from left to right. The index in the array corresponds to the index used in selectedScopeButtonIndex.

## See Also

### Configuring scope bar buttons

var selectedScopeButtonIndex: Int

The index of the selected scope button.

var showsScopeBar: Bool

Specifies whether the scope bar is displayed.

func setShowsScope(Bool, animated: Bool)

Specifies whether the scope bar is displayed, optionally using an animation.

