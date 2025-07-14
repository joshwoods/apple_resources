

- AppKit
- NSColorPickerTouchBarItem
-  colorPicker(withIdentifier:) 

Type Method

# colorPicker(withIdentifier:)

Creates a bar item with the standard color picker icon.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

``` source
@MainActor
class func colorPicker(withIdentifier identifier: NSTouchBarItem.Identifier) -> Self
```

## See Also

### Creating a color picker item

class func textColorPicker(withIdentifier: NSTouchBarItem.Identifier) -> Self

Creates a bar item with the standard text color picker icon.

class func strokeColorPicker(withIdentifier: NSTouchBarItem.Identifier) -> Self

Creates a bar item with the standard stroke color picker icon.

class func colorPicker(withIdentifier: NSTouchBarItem.Identifier, buttonImage: UIImage) -> Self

Creates a color picker bar item using the supplied image as its icon.

