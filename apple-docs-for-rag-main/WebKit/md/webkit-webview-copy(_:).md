

- WebKit
- WebView
-  copy(\_:) 

Instance Method

# copy(\_:)

Action method that copies the selected content to the general pasteboard.

macOS

``` source
@MainActor
func copy(_ sender: Any?)
```

## Parameters 

`sender`  

The object that sent this message.

## Discussion

This action method copies the selected content onto the general pasteboard, in as many formats as the receiver supports. For example, a plain text object uses `NSStringPboardType` for plain text, and a rich text object also uses `NSRTFPboardType`.

## See Also

### Cut, Copy and Paste Action Methods

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

func pasteAsRichText(Any?)

An action method that pastes pasteboard content into the receiver as rich text, maintaining its attributes.

