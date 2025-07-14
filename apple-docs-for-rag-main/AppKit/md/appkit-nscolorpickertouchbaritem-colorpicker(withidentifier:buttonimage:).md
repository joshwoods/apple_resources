

- AppKit
- NSColorPickerTouchBarItem
-  colorPicker(withIdentifier:buttonImage:) 

Type Method

# colorPicker(withIdentifier:buttonImage:)

Creates a color picker bar item using the supplied image as its icon.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

**macOS**

``` source
@MainActor
class func colorPicker(
    withIdentifier identifier: NSTouchBarItem.Identifier,
    buttonImage image: NSImage
) -> Self
```

**Mac Catalyst**

``` source
@MainActor
class func colorPicker(
    withIdentifier identifier: NSTouchBarItem.Identifier,
    buttonImage image: UIImage
) -> Self
```

## See Also

### Creating a color picker item

class func colorPicker(withIdentifier: NSTouchBarItem.Identifier) -> Self

Creates a bar item with the standard color picker icon.

class func textColorPicker(withIdentifier: NSTouchBarItem.Identifier) -> Self

Creates a bar item with the standard text color picker icon.

class func strokeColorPicker(withIdentifier: NSTouchBarItem.Identifier) -> Self

Creates a bar item with the standard stroke color picker icon.

