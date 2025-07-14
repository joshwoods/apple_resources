

- UIKit
- UIResponderStandardEditActions
-  paste(\_:) 

Instance Method

# paste(\_:)

Pastes the current contents of the pasteboard into your app’s interface.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func paste(_ sender: Any?)
```

## Parameters 

`sender`  

The object calling this method.

## Mentioned in 

Using responders and the responder chain to handle events

## Discussion

UIKit calls this method when the user selects the Paste command from an editing menu. Your implementation should read the data from the pasteboard and add the resulting content to your interface.

## See Also

### Handling copy, cut, paste, and delete commands

func cut(Any?)

Removes the selected content and writes the data for it to the pasteboard.

func copy(Any?)

Copies the selected content to the pasteboard.

func pasteAndGo(Any?)

Pastes the current contents of the pasteboard into your app’s interface and navigates to the entity it references.

func pasteAndMatchStyle(Any?)

Pastes the current contents of the pasteboard into your app’s interface using the text style of the target.

func pasteAndSearch(Any?)

Pastes the current contents of the pasteboard into your app’s interface and performs a search.

func delete(Any?)

Removes the selected content from your interface.

