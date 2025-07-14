

- UIKit
- UIFindInteraction
-  delegate 

Instance Property

# delegate

An object that updates your app’s presentation and provides the session object for managing the interaction’s search.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any UIFindInteractionDelegate)? { get }
```

## See Also

### Managing find interactions

func presentFindNavigator(showingReplace: Bool)

Begins a search, displaying the find panel.

func dismissFindNavigator()

Dismisses the find panel, if present.

func findNext()

Highlights the next found result in the content, relative to the currently highlighted result.

func findPrevious()

Highlights the previously found result in the document, relative to the currently highlighted result.

