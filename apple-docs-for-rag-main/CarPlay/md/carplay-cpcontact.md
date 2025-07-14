

- CarPlay
-  CPContact 

Class

# CPContact

A data object that contains information about a contact.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class CPContact
```

## Overview

`CPContact` is an object that represents information about a person or a business, and can include a set of contextually relevant actions that a user can perform when CarPlay displays the contact, such as getting directions to its location.

You display a contact using CPContactTemplate. The template manages the appearance of the contact, and can display up to four action buttons. After displaying it, you can update the buttons for the template by assigning a new array to the contact’s actions property.

The framework provides specialized buttons for common actions, such as CPContactCallButton or CPContactMessageButton.

## Topics

### Creating a Contact

init(name: String, image: UIImage)

Creates a contact with a name and an image.

### Configuring the Contact’s Attributes

var image: UIImage

The contact’s image.

var name: String

The contact’s name.

var subtitle: String?

A subtitle that the template displays in addition to the contact’s name.

var informativeText: String?

Additional text that the template displays.

### Managing Interactions with the Contact

var actions: [CPButton]?

The actions that the template displays for this contact.

class CPContactCallButton

A button for calling the contact.

class CPContactDirectionsButton

A button for getting directions to the contact’s location.

class CPContactMessageButton

A button that activates Siri and initiates the compose message flow.

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

### Configuring the Contact

var contact: CPContact

The contact that the template displays.

