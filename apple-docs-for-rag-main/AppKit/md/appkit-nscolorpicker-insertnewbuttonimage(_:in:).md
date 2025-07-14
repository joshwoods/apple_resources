

- AppKit
- NSColorPicker
-  insertNewButtonImage(\_:in:) 

Instance Method

# insertNewButtonImage(\_:in:)

Sets the image used for the specified button cell.

macOS

``` source
@MainActor
func insertNewButtonImage(
    _ newButtonImage: NSImage,
    in buttonCell: NSButtonCell
)
```

## Parameters 

`newButtonImage`  

The image used for the specified button cell.

`buttonCell`  

The button cell for which to set the image.

## Discussion

Called by the color panel to insert a new image into the specified cell by invoking `NSButtonCell`’s setImage: method. Override this method to customize `newButtonImage` before insertion in `buttonCell`.

## See Also

### Adding Button Images

var provideNewButtonImage: NSImage

The button image used by the color picker.

