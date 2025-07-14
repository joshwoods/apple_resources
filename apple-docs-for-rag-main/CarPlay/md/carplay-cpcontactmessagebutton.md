

- CarPlay
-  CPContactMessageButton 

Class

# CPContactMessageButton

A button that activates Siri and initiates the compose message flow.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class CPContactMessageButton
```

## Overview

Important

This subclass of CPButton doesn’t use a handler. Instead, tapping this button activates Siri and launches the compose message flow using the contact information in the phoneOrEmail property.

## Topics

### Creating a Contact Message Button

init(phoneOrEmail: String)

Creates a contact message button with the provided contact information.

### Getting the Contact Information

var phoneOrEmail: String

The contact’s phone number or email address.

## Relationships

### Inherits From

- CPButton

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Managing Interactions with the Contact

var actions: [CPButton]?

The actions that the template displays for this contact.

class CPContactCallButton

A button for calling the contact.

class CPContactDirectionsButton

A button for getting directions to the contact’s location.

