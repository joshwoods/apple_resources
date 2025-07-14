

- CarPlay
-  CPMapButton 

Class

# CPMapButton

A button that represents an action that a map template displays on the CarPlay screen.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
class CPMapButton
```

## Topics

### Creating a Map Button

init(handler: ((CPMapButton) -> Void)?)

Creates a new map button.

### Providing Button Images

var image: UIImage?

The image to display on the button.

var focusedImage: UIImage?

The image to display when focus is on the button.

### Controlling the Button

var isEnabled: Bool

A Boolean value that enables and disables the map button.

var isHidden: Bool

A Boolean value that hides and shows the map button.

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

### Managing Map Buttons

var mapButtons: [CPMapButton]

An array of map buttons on the trailing bottom corner of the map template.

