

- CarPlay
-  CPGridButton 

Class

# CPGridButton

A menu item button displayed on a grid template.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
class CPGridButton
```

## Topics

### Creating a Grid Button

init(titleVariants: [String], image: UIImage, handler: ((CPGridButton) -> Void)?)

Creates a grid button with the specified title variants, image, and action handler.

### Controlling the Grid Button

var isEnabled: Bool

A Boolean value that enables and disables the grid button.

### Obtaining Grid Button Information

var titleVariants: [String]

An array of title variants for the button.

var image: UIImage

The image displayed on the button.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Creating a Grid Template

init(title: String?, gridButtons: [CPGridButton])

Creates a grid template with a title and a set of buttons.

