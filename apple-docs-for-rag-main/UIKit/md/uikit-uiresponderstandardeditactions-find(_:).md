

- UIKit
- UIResponderStandardEditActions
-  find(\_:) 

Instance Method

# find(\_:)

Begins a search for content in your app’s interface.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
@MainActor
optional func find(_ sender: Any?)
```

## Parameters 

`sender`  

The object calling this method.

## Discussion

UIKit calls this method when the user selects the Find command from an editing menu. Your implementation should present the UI for finding textual content in your view.

For example, a view using a find interaction might call presentFindNavigator(showingReplace:) to present the system find panel.

## See Also

### Handling find and replace commands

func findNext(Any?)

Finds the next match in your app’s interface.

func findPrevious(Any?)

Finds the previous match in your app’s interface.

func findAndReplace(Any?)

Begins a search for content in your app’s interface and provides a replacement.

func useSelectionForFind(Any?)

Begins a search for the selected content in your app’s interface.

