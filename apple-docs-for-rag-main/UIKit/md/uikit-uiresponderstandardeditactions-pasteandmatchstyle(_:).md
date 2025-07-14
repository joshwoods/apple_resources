

- UIKit
- UIResponderStandardEditActions
-  pasteAndMatchStyle(\_:) 

Instance Method

# pasteAndMatchStyle(\_:)

Pastes the current contents of the pasteboard into your app’s interface using the text style of the target.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
@MainActor
optional func pasteAndMatchStyle(_ sender: Any?)
```

## Parameters 

`sender`  

The object calling this method.

## Discussion

UIKit calls this method when the user selects the Paste command from an editing menu. Your implementation should read the data from the pasteboard and add the resulting content to your interface using the target’s current text style.

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

func pasteAndSearch(Any?)

Pastes the current contents of the pasteboard into your app’s interface and performs a search.

func delete(Any?)

Removes the selected content from your interface.

