

- UIKit
- UIFindInteraction
-  findPrevious() 

Instance Method

# findPrevious()

Highlights the previously found result in the document, relative to the currently highlighted result.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
func findPrevious()
```

## See Also

### Managing find interactions

var delegate: (any UIFindInteractionDelegate)?

An object that updates your app’s presentation and provides the session object for managing the interaction’s search.

func presentFindNavigator(showingReplace: Bool)

Begins a search, displaying the find panel.

func dismissFindNavigator()

Dismisses the find panel, if present.

func findNext()

Highlights the next found result in the content, relative to the currently highlighted result.

