

- CarPlay
-  CPContactTemplate 

Class

# CPContactTemplate

A template that displays information about a person or a business.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class CPContactTemplate
```

## Overview

The contact template can provide up to four contextual actions a user can invoke. For example, you might have an action that provides directions to the contact’s address.

When creating a contact template, you provide an instance of CPContact that contains a contact’s name and image, and optional subtitle. The object also contains any actions relevant to the contact. CarPlay provides specialized buttons for common actions, such as CPContactCallButton or CPContactMessageButton.

To display a contact template, call your interface controller’s pushTemplate(_:animated:completion:) method to push it onto the navigation hierarchy, or presentTemplate(_:animated:completion:) to present it modally.

Note

`CPContactTemplate` is only available in apps that have the communication or navigation entitlements.

## Topics

### Creating a Contact Template

init(contact: CPContact)

Creates a contact template that displays the provided contact.

### Configuring the Contact

var contact: CPContact

The contact that the template displays.

class CPContact

A data object that contains information about a contact.

## Relationships

### Inherits From

- CPTemplate

### Conforms To

- CPBarButtonProviding
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

