

- Contacts
-  CNContactsUserDefaults 

Class

# CNContactsUserDefaults

An object that defines the default options to use when displaying contacts.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
class CNContactsUserDefaults
```

## Topics

### Getting the Shared Database

class func shared() -> Self

The singleton contacts user defaults object.

### Getting the Default Values

var countryCode: String

An ISO country code.

var sortOrder: CNContactSortOrder

Default sorting order by name.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Formatters

class CNContactFormatter

An object that you use to format contact information before displaying it to the user.

class CNPostalAddressFormatter

An object that you use to format a contact’s postal addresses.

class CNContactVCardSerialization

An object you use to convert to and from a vCard representation of the user’s contacts.

