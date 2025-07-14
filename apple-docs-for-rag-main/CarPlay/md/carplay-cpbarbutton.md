

- CarPlay
-  CPBarButton 

Class

# CPBarButton

A button for placement in a navigation bar.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
class CPBarButton
```

## Topics

### Creating a CarPlay Bar Button

init?(coder: NSCoder)

Creates a button initialized from data in the specified coder object.

init(type: CPBarButton.Type, handler: CPBarButtonHandler?)

Creates a bar button with a type and handler.

Deprecated

init(image: UIImage, handler: CPBarButtonHandler?)

Creates a bar button that displays an image.

init(title: String, handler: CPBarButtonHandler?)

Creates a bar button that displays a text label.

enum Type

Types of bar buttons.

typealias CPBarButtonHandler

A block that CarPlay calls when the user taps a bar button.

### Configuring the Button

var isEnabled: Bool

A Boolean value that enables and disables the bar button.

var image: UIImage?

The image displayed on the bar button.

var title: String?

The title displayed on the bar button.

### Getting the Button Style

var buttonType: CPBarButton.Type

The display type for the bar button.

Deprecated

var buttonStyle: CPBarButtonStyle

The style to use when displaying the button.

enum CPBarButtonStyle

The display style of a bar button.

## Relationships

### Inherits From

- NSObject

### Inherited By

- CPMessageComposeBarButton

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

### Providing Navigation Bar Buttons

var backButton: CPBarButton?

A button to display as the Back button on the navigation bar.

**Required**

var leadingNavigationBarButtons: [CPBarButton]

An array of bar buttons to display on the leading side of the navigation bar.

**Required**

var trailingNavigationBarButtons: [CPBarButton]

An array of bar buttons to display on the trailing side of the navigation bar.

**Required**

class CPMessageComposeBarButton

A button that activates Siri and initiates the compose message flow.

