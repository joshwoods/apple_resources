

- CarPlay
-  CPMessageComposeBarButton 

Class

# CPMessageComposeBarButton

A button that activates Siri and initiates the compose message flow.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class CPMessageComposeBarButton
```

## Overview

Note

This button type does not use a handler. Instead, tapping this button activates Siri and initiates the compose message flow.

## Topics

### Creating a Message Compose Bar Button

init()

Creates a message compose button with a system-provided image.

init(image: UIImage)

Creates a message compose button that displays a custom image.

## Relationships

### Inherits From

- CPBarButton

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

class CPBarButton

A button for placement in a navigation bar.

