

- Contacts
-  CNContactFormatter 

Class

# CNContactFormatter

An object that you use to format contact information before displaying it to the user.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
class CNContactFormatter
```

## Overview

A `CNContactFormatter` object handles international ordering and delimiting for the contact name components. When formatting many contacts, create an instance of this class and use the instance methods; otherwise use the class methods.

## Topics

### Creating a formatted attributed string

func attributedString(from: CNContact, defaultAttributes: [AnyHashable : Any]?) -> NSAttributedString?

Formats the contact name as an attributed string.

class func attributedString(from: CNContact, style: CNContactFormatterStyle, defaultAttributes: [AnyHashable : Any]?) -> NSAttributedString?

Formats the contact name as an attributed string.

### Creating a formatted string

func string(from: CNContact) -> String?

Formats the contact name.

class func string(from: CNContact, style: CNContactFormatterStyle) -> String?

Returns the contact name, formatted with the specified formatter.

### Specifying the formatting style

var style: CNContactFormatterStyle

The formatting style for the contact name.

enum CNContactFormatterStyle

The formatting styles for contact names.

### Getting a descriptor

class func descriptorForRequiredKeys(for: CNContactFormatterStyle) -> any CNKeyDescriptor

Returns the required key descriptor for the specified formatting style of the contact.

class var descriptorForRequiredKeysForDelimiter: any CNKeyDescriptor

Returns the required key descriptor for the name delimiter.

class var descriptorForRequiredKeysForNameOrder: any CNKeyDescriptor

Returns the required key descriptor for the display name order.

### Getting format information

class func delimiter(for: CNContact) -> String

Returns the delimiter to use between name components.

class func nameOrder(for: CNContact) -> CNContactDisplayNameOrder

Returns the display name order.

enum CNContactDisplayNameOrder

The formatting orders for contact names component.

## Relationships

### Inherits From

- Formatter

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Formatters

class CNPostalAddressFormatter

An object that you use to format a contact’s postal addresses.

class CNContactVCardSerialization

An object you use to convert to and from a vCard representation of the user’s contacts.

class CNContactsUserDefaults

An object that defines the default options to use when displaying contacts.

