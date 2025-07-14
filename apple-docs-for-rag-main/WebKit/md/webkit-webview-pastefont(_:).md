

- WebKit
- WebView
-  pasteFont(\_:) 

Instance Method

# pasteFont(\_:)

An action method that pastes font information from the font pasteboard.

macOS

``` source
@MainActor
func pasteFont(_ sender: Any?)
```

## Parameters 

`sender`  

The object that sent this message.

## Discussion

This action method pastes font information from the font pasteboard onto the selected content or insertion point of a rich text object, or over all text of the receiver.

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

func pasteAsPlainText(Any?)

An action method that pastes pasteboard content as plain text.

func pasteAsRichText(Any?)

An action method that pastes pasteboard content into the receiver as rich text, maintaining its attributes.

