

- Address Book
-  ABRecord 

Class

# ABRecord

An abstract class that defines the common properties for all Address Book records.

macOS

``` source
class ABRecord
```

## Overview

`ABRecord` is an abstract superclass providing a common interface to, and defining common properties for, all Address Book records. A property is a field in the database record, such as the first or last name of a person record. ABRecord defines the types of properties supported, and basic methods for getting, setting, and removing property values.

The `ABRecord` class is “toll-free bridged” with its procedural C opaque-type counterpart. This means that the `ABRecordRef` type is interchangeable in function or method calls with instances of the `ABRecord` class.

## Topics

### Creating a Record

init!(addressBook: ABAddressBook!)

Initializes a record using the given address book.

init!()

Initializes a record using the shared address book.

### Retrieving and Setting Values

func removeValue(forProperty: String!) -> Bool

Removes the value for a given property.

func setValue(Any!, forProperty: String!) -> Bool

Sets the value of a given property for a record.

func setValue(Any!, forProperty: String!, error: ()) throws

Sets the value of a given property for a record, returning error information.

func value(forProperty: String!) -> Any!

Returns the value of a given property for a record.

### Retrieving a Specific Record

func isReadOnly() -> Bool

Returns whether a record is read-only.

### Getting Identifying Information

var displayName: String!

A user-visible string representing the record.

var uniqueId: String!

Returns the unique ID for a record.

## Relationships

### Inherits From

- NSObject

### Inherited By

- ABGroup
- ABPerson

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Data Types

class ABPerson

An object that encapsulates all information about a person in the Address Book database.

class ABGroup

An object that represents a group of records in the Address Book database.

class ABMultiValue

An immutable representation of a property that might have multiple values.

class ABMutableMultiValue

A mutable representation of a property that might have multiple values.

protocol ABImageClient

Methods for responding to a request to load images associated with a contact.

