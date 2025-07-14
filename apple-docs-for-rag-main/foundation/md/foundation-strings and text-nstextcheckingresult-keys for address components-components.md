

- Foundation
- Strings and Text
- NSTextCheckingResult
-  Keys for Address Components 

API Collection

# Keys for Address Components

The following constants identify the possible keys returned in the addressComponents dictionary.

## Topics

### Constants

static let name: NSTextCheckingKey

A key that corresponds to the name component of the address.

static let jobTitle: NSTextCheckingKey

A key that corresponds to the job component of the address.

static let organization: NSTextCheckingKey

A key that corresponds to the organization component of the address.

static let street: NSTextCheckingKey

A key that corresponds to the street address component of the address.

static let city: NSTextCheckingKey

A key that corresponds to the city component of the address.

static let state: NSTextCheckingKey

A key that corresponds to the state or province component of the address.

static let zip: NSTextCheckingKey

A key that corresponds to the zip code or postal code component of the address.

static let country: NSTextCheckingKey

A key that corresponds to the country or region component of the address.

static let phone: NSTextCheckingKey

A key that corresponds to the phone number component of the address.

## See Also

### Constants

Keys for Transit Components

The following constants identify the possible keys returned in the components dictionary.

struct CheckingType

These constants specify the type of checking the methods should do. They are returned by resultType.

typealias NSTextCheckingTypes

Defines the types of checking that are available. These values can be combined using the C-bitwise OR operator. The system supports its own internal types, and the user can extend those types by subclassing `NSTextCheckingResult` and adding their own custom types.

struct NSTextCheckingKey

Anonymous

