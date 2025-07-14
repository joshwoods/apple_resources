

- UIKit
- UIFindInteraction
-  isFindNavigatorVisible 

Instance Property

# isFindNavigatorVisible

A Boolean value that indicates when the find panel displays onscreen.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var isFindNavigatorVisible: Bool { get }
```

## Discussion

The value of this property is `YES` when the find panel displays; otherwise, `NO`.

## See Also

### Configuring the find panel

var searchText: String?

The search query with which to prepopulate the find panel’s search text field.

var replacementText: String?

The replacement string with which to prepopulate the find panel’s replace text field.

var optionsMenuProvider: (([UIMenuElement]) -> UIMenu?)?

A closure that populates the search options for a find interaction.

