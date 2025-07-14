

- UIKit
- UIResponderStandardEditActions
-  pasteAndSearch(\_:) 

Instance Method

# pasteAndSearch(\_:)

Pastes the current contents of the pasteboard into your app’s interface and performs a search.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
@MainActor
optional func pasteAndSearch(_ sender: Any?)
```

## Parameters 

`sender`  

The object calling this method.

## Discussion

UIKit calls this method when the user selects the Paste and Search command from an editing menu. Your implementation should read the data from the pasteboard and begin a search based on the content.

## See Also

### Handling copy, cut, paste, and delete commands

func cut(Any?)

Removes the selected content and writes the data for it to the pasteboard.

func copy(Any?)

Copies the selected content to the pasteboard.

func paste(Any?)

Pastes the current contents of the pasteboard into your app’s interface.

func pasteAndGo(Any?)

Pastes the current contents of the pasteboard into your app’s interface and navigates to the entity it references.

func pasteAndMatchStyle(Any?)

Pastes the current contents of the pasteboard into your app’s interface using the text style of the target.

func delete(Any?)

Removes the selected content from your interface.

