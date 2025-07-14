

- UIKit
- UISearchBar
-  selectedScopeButtonIndex 

Instance Property

# selectedScopeButtonIndex

The index of the selected scope button.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var selectedScopeButtonIndex: Int { get set }
```

## Discussion

The indexes of the scope buttons are determined by the indexes of the strings in scopeButtonTitles.

## See Also

### Configuring scope bar buttons

var scopeButtonTitles: [String]?

An array of strings indicating the titles of the scope buttons.

var showsScopeBar: Bool

Specifies whether the scope bar is displayed.

func setShowsScope(Bool, animated: Bool)

Specifies whether the scope bar is displayed, optionally using an animation.

