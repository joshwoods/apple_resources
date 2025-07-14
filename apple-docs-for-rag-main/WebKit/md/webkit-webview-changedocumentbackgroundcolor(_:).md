

- WebKit
- WebView
-  changeDocumentBackgroundColor(\_:) 

Instance Method

# changeDocumentBackgroundColor(\_:)

Sets the background color of the selected content.

macOS

``` source
@MainActor
func changeDocumentBackgroundColor(_ sender: Any?)
```

## Parameters 

`sender`  

The object that sent this message.

## Discussion

This method is invoked by the `NSColorPanel` sender and behaves similar to the changeDocumentBackgroundColor(_:) method in NSTextView.

## See Also

### Changing the Font, Color and Other Attributes When Editing

func changeFont(Any?)

An action method that changes the font of the selection, or all content if there is no selection.

func changeAttributes(Any?)

An action method that changes the attributes of the current selection.

func changeColor(Any?)

Sets the color of the selected content.

