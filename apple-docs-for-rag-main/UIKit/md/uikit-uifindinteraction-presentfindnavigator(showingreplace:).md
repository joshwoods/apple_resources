

- UIKit
- UIFindInteraction
-  presentFindNavigator(showingReplace:) 

Instance Method

# presentFindNavigator(showingReplace:)

Begins a search, displaying the find panel.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
func presentFindNavigator(showingReplace: Bool)
```

## Parameters 

`showingReplace`  

`YES` to display a replace text field in the panel if the delegate supports text replacement. `No` to avoid displaying the replace text field.

## Discussion

You use this method to begin a search and display the find panel. The method calls findInteraction(_:sessionFor:) on the interaction object’s delegate and updates the UI using the session object the delegate returns.

The following example presents the find panel from a bar button item.

```
@objc func findButtonTapped(sender: UIBarButtonItem) {
    self.findInteraction!.presentFindNavigator(showingReplace: false)
}
```

The method has no effect if the find navigator panel is already present.

## See Also

### Managing find interactions

var delegate: (any UIFindInteractionDelegate)?

An object that updates your app’s presentation and provides the session object for managing the interaction’s search.

func dismissFindNavigator()

Dismisses the find panel, if present.

func findNext()

Highlights the next found result in the content, relative to the currently highlighted result.

func findPrevious()

Highlights the previously found result in the document, relative to the currently highlighted result.

