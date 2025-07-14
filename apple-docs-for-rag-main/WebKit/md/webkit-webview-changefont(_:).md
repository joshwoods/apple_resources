

- WebKit
- WebView
-  changeFont(\_:) 

Instance Method

# changeFont(\_:)

An action method that changes the font of the selection, or all content if there is no selection.

macOS

``` source
@MainActor
func changeFont(_ sender: Any?)
```

## Parameters 

`sender`  

The object that sent this message.

## Discussion

If the receiver doesn’t use the Fonts panel, this method does nothing.

## See Also

### Changing the Font, Color and Other Attributes When Editing

func changeAttributes(Any?)

An action method that changes the attributes of the current selection.

func changeDocumentBackgroundColor(Any?)

Sets the background color of the selected content.

func changeColor(Any?)

Sets the color of the selected content.

