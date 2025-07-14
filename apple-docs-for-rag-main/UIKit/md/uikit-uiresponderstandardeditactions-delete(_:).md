

- UIKit
- UIResponderStandardEditActions
-  delete(\_:) 

Instance Method

# delete(\_:)

Removes the selected content from your interface.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func delete(_ sender: Any?)
```

## Parameters 

`sender`  

The object calling this method.

## Discussion

UIKit calls this method when the user selects the Delete command from an editing menu. Your implementation should remove the selected content from your interface.

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

func pasteAndSearch(Any?)

Pastes the current contents of the pasteboard into your app’s interface and performs a search.

