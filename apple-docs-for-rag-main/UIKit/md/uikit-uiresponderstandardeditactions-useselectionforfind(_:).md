

- UIKit
- UIResponderStandardEditActions
-  useSelectionForFind(\_:) 

Instance Method

# useSelectionForFind(\_:)

Begins a search for the selected content in your app’s interface.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
@MainActor
optional func useSelectionForFind(_ sender: Any?)
```

## Parameters 

`sender`  

The object calling this method.

## Discussion

UIKit calls this method when the user selects the Use Selection For Find command from an editing menu. Your implementation should present the UI for finding textual content in your view and use the selected text for the search.

For example, a view using a find interaction might call presentFindNavigator(showingReplace:) and pass the selected text as the query string.

## See Also

### Handling find and replace commands

func find(Any?)

Begins a search for content in your app’s interface.

func findNext(Any?)

Finds the next match in your app’s interface.

func findPrevious(Any?)

Finds the previous match in your app’s interface.

func findAndReplace(Any?)

Begins a search for content in your app’s interface and provides a replacement.

