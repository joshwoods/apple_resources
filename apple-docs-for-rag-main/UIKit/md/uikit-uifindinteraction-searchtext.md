

- UIKit
- UIFindInteraction
-  searchText 

Instance Property

# searchText

The search query with which to prepopulate the find panel’s search text field.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var searchText: String? { get set }
```

## See Also

### Configuring the find panel

var isFindNavigatorVisible: Bool

A Boolean value that indicates when the find panel displays onscreen.

var replacementText: String?

The replacement string with which to prepopulate the find panel’s replace text field.

var optionsMenuProvider: (([UIMenuElement]) -> UIMenu?)?

A closure that populates the search options for a find interaction.

