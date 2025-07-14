

- UIKit
- UISearchBar
-  showsScopeBar 

Instance Property

# showsScopeBar

Specifies whether the scope bar is displayed.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var showsScopeBar: Bool { get set }
```

## Discussion

If the search bar is owned by a UISearchController, then setting this property implicitly sets the search controller’s automaticallyShowsScopeBar property to false.

## See Also

### Configuring scope bar buttons

var scopeButtonTitles: [String]?

An array of strings indicating the titles of the scope buttons.

var selectedScopeButtonIndex: Int

The index of the selected scope button.

func setShowsScope(Bool, animated: Bool)

Specifies whether the scope bar is displayed, optionally using an animation.

