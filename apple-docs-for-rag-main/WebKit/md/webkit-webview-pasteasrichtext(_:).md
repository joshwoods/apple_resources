

- WebKit
- WebView
-  pasteAsRichText(\_:) 

Instance Method

# pasteAsRichText(\_:)

An action method that pastes pasteboard content into the receiver as rich text, maintaining its attributes.

macOS

``` source
@MainActor
func pasteAsRichText(_ sender: Any?)
```

## Parameters 

`sender`  

The object that sent this message.

## Discussion

The text is inserted at the insertion point if there is one; otherwise, it replaces the selection.

## See Also

### Cut, Copy and Paste Action Methods

func copy(Any?)

Action method that copies the selected content to the general pasteboard.

func copyFont(Any?)

An action method that copies font information onto the font pasteboard.

func cut(Any?)

An action method that deletes selected content and puts it on the general pasteboard.

func delete(Any?)

An action method that deletes the selected content.

func paste(Any?)

An action method that pastes content from the pasteboard at the insertion point or over the selection.

func pasteFont(Any?)

An action method that pastes font information from the font pasteboard.

func pasteAsPlainText(Any?)

An action method that pastes pasteboard content as plain text.

