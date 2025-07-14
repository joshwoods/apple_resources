

- WebKit
- WebView
-  changeAttributes(\_:) 

Instance Method

# changeAttributes(\_:)

An action method that changes the attributes of the current selection.

macOS

``` source
@MainActor
func changeAttributes(_ sender: Any?)
```

## Parameters 

`sender`  

The object that sent this message.

## Discussion

This method behaves similar to the changeAttributes(_:) method in NSTextView.

## See Also

### Changing the Font, Color and Other Attributes When Editing

func changeFont(Any?)

An action method that changes the font of the selection, or all content if there is no selection.

func changeDocumentBackgroundColor(Any?)

Sets the background color of the selected content.

func changeColor(Any?)

Sets the color of the selected content.

