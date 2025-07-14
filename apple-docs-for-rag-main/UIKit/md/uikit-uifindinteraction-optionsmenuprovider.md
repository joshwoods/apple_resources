

- UIKit
- UIFindInteraction
-  optionsMenuProvider 

Instance Property

# optionsMenuProvider

A closure that populates the search options for a find interaction.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var optionsMenuProvider: (([UIMenuElement]) -> UIMenu?)? { get set }
```

## Discussion

You use this closure to modify, augement or omit options from the default set available in UITextSearchOptions.

## See Also

### Configuring the find panel

var isFindNavigatorVisible: Bool

A Boolean value that indicates when the find panel displays onscreen.

var searchText: String?

The search query with which to prepopulate the find panel’s search text field.

var replacementText: String?

The replacement string with which to prepopulate the find panel’s replace text field.

