

- CarPlay
-  CPDashboardButton 

Class

# CPDashboardButton

A shortcut button for placement on the CarPlay Dashboard.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+

``` source
class CPDashboardButton
```

## Topics

### Creating a Dashboard Button

init(titleVariants: [String], subtitleVariants: [String], image: UIImage, handler: ((CPDashboardButton) -> Void)?)

Creates a dashboard button that displays a title, an optional subtitle, and an image.

### Accessing the Button Configuration

var titleVariants: [String]

The array of title variants for the button.

var subtitleVariants: [String]

The array of subtitle variants for the button.

var image: UIImage

The image the button displays.

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

### Providing Dashboard Buttons

var shortcutButtons: [CPDashboardButton]

An array of shortcut buttons to display on the CarPlay Dashboard.

