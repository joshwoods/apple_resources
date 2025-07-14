

- AppKit
- NSColorPicker
-  provideNewButtonImage 

Instance Property

# provideNewButtonImage

The button image used by the color picker.

macOS

``` source
var provideNewButtonImage: NSImage { get }
```

## Discussion

The image placed on the mode button the user uses to select this color picker. This is the same image the color panel uses as an argument when sending the insertNewButtonImage(_:in:) message. Override this property’s getter method to provide a custom button image. The default implementation looks in the color picker’s bundle for a TIFF file named after the color picker’s class, with the extension “`.tiff`”.

## See Also

### Adding Button Images

func insertNewButtonImage(NSImage, in: NSButtonCell)

Sets the image used for the specified button cell.

