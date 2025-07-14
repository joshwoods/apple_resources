

- UIKit
- UIFindInteraction
-  replacementText 

Instance Property

# replacementText

The replacement string with which to prepopulate the find panel’s replace text field.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var replacementText: String? { get set }
```

## See Also

### Configuring the find panel

var isFindNavigatorVisible: Bool

A Boolean value that indicates when the find panel displays onscreen.

var searchText: String?

The search query with which to prepopulate the find panel’s search text field.

var optionsMenuProvider: (([UIMenuElement]) -> UIMenu?)?

A closure that populates the search options for a find interaction.

