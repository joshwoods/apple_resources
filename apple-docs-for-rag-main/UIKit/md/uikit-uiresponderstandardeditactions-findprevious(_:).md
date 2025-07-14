

- UIKit
- UIResponderStandardEditActions
-  findPrevious(\_:) 

Instance Method

# findPrevious(\_:)

Finds the previous match in your app’s interface.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
@MainActor
optional func findPrevious(_ sender: Any?)
```

## Parameters 

`sender`  

The object calling this method.

## Discussion

UIKit calls this method when the user selects the Find Previous command from an editing menu. Your implementation should highlight the previous result in the UI for finding textual content in your view.

For example, a view using a find interaction might call highlightNextResult(in:) to update the find session.

## See Also

### Handling find and replace commands

func find(Any?)

Begins a search for content in your app’s interface.

func findNext(Any?)

Finds the next match in your app’s interface.

func findAndReplace(Any?)

Begins a search for content in your app’s interface and provides a replacement.

func useSelectionForFind(Any?)

Begins a search for the selected content in your app’s interface.

