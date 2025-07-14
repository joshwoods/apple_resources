

- Contacts
-  CNContactProperty 

Class

# CNContactProperty

An object that represents a property of a contact.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
class CNContactProperty
```

## Overview

A contact (that is, an instance of CNContact) has properties, such as givenName, phoneNumbers, and jobTitle. Each property is represented by an instance of CNContactProperty, which provides a tuple that can contain three or five values, depending on whether the property is a member of an array of labeled values. For example, the phoneNumbers property is a member of an array of labeled values, so the `CNContactProperty` tuple contains the contact, key, value, identifier, and label. For the givenName property, which is not contained in a labeled array, `CNContactProperty` returns a tuple that contains the contact, key, and value. The `CNContactProperty` class is used by CNContactPicker to return the user’s selected property.

## Topics

### Getting the Contact Object

var contact: CNContact

The associated contact.

### Getting the Property Information

var key: String

The key of the contact property.

var value: Any?

The value of the property.

var label: String?

The label of the labeled value of the property array.

var identifier: String?

The identifier of the labeled value in the array of labeled.

### Handling Exceptions

let CNContactPropertyNotFetchedExceptionName: String

Exception thrown when an accessed property was not fetched.

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
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Generic Types

class CNLabeledValue

An immutable object that combines a contact property value with a label that describes that property.

