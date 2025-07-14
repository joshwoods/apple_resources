

- Contacts
-  CNPhoneNumber 

Class

# CNPhoneNumber

An immutable object representing a phone number for a contact.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
class CNPhoneNumber
```

## Overview

`CNPhoneNumber` objects are thread-safe, and you may access their properties from any thread of your app.

## Topics

### Creating a Phone Number Object

init(stringValue: String)

Returns a new phone number object initialized with the specified phone number string.

### Getting the Phone Number

var stringValue: String

The string value of the phone number.

### Getting Phone-Related Keys

let CNContactPhoneNumbersKey: String

A phone numbers of a contact.

### Deprecated

init!()Deprecated

class func new() -> Self!Deprecated

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

