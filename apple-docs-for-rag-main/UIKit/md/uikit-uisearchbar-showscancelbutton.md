

- UIKit
- UISearchBar
-  showsCancelButton 

Instance Property

# showsCancelButton

A Boolean value indicating whether the cancel button is displayed.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var showsCancelButton: Bool { get set }
```

## Discussion

When the value of this property is true, the cancel button is displayed if the app is running on iPhone. The value of this property is ignored, and no cancel button is displayed, for apps running on iPad. The default value is false.

## See Also

### Configuring the search interface

var showsBookmarkButton: Bool

A Boolean value indicating whether the bookmark button is displayed.

func setShowsCancelButton(Bool, animated: Bool)

Sets the display state of the cancel button optionally with animation.

var showsSearchResultsButton: Bool

A Boolean value indicating whether the search results button is displayed.

var isSearchResultsButtonSelected: Bool

A Boolean value indicating whether the search results button is selected.

