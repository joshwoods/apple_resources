

- Address Book
-  ABPerson 

Class

# ABPerson

An object that encapsulates all information about a person in the Address Book database.

macOS

``` source
class ABPerson
```

## Overview

An `ABPerson` object corresponds to a single person record in the database. A person object contains the person’s name, company, address, email addresses, and phone numbers.

The `ABPerson` class is “toll-free bridged” with its procedural C opaque-type counterpart. This means that the `ABPersonRef` type is interchangeable in function or method calls with instances of the `ABPerson` class.

## Topics

### Managing Properties

class func addPropertiesAndTypes([AnyHashable : Any]!) -> Int

Adds the given properties to all the records of this type in the Address Book database.

class func removeProperties([Any]!) -> Int

Removes the given properties from all the records of this type in the Address Book database.

class func properties() -> [Any]!

Returns an array of the names of all the properties for the record in the Address Book database.

class func type(ofProperty: String!) -> ABPropertyType

Returns the type of a given property.

### Managing Linked People

func linkedPeople() -> [Any]!

Returns the array of all person records that are linked to the person this record represents.

### Managing Groups

func parentGroups() -> [Any]!

Returns an array of the address book groups that this person belongs to.

### Managing Images

class func cancelLoadingImageData(forTag: Int)

Cancels an asynchronous fetch of the images for a given tag.

func beginLoadingImageData(for: (any ABImageClient)!) -> Int

Starts an asynchronous fetch for image data in all locations

func imageData() -> Data!

Returns data that contains a picture of this person.

func setImageData(Data!) -> Bool

Sets the image for this person to the given data.

### Searching

class func searchElement(forProperty: String!, label: String!, key: String!, value: Any!, comparison: ABSearchComparison) -> ABSearchElement!

Returns a search element object that specifies a query for records of this type.

### Importing and Exporting vCard Formatted Files

init!(VCardRepresentation: Data!)

Returns an `ABPerson` instance initialized with the given data.

func vCardRepresentation() -> Data!

Returns the vCard representation of the person record as a data object in vCard format.

### Constants

Person Flags

Settings that determine how person records are displayed.

## Relationships

### Inherits From

- ABRecord

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Data Types

class ABGroup

An object that represents a group of records in the Address Book database.

class ABMultiValue

An immutable representation of a property that might have multiple values.

class ABMutableMultiValue

A mutable representation of a property that might have multiple values.

protocol ABImageClient

Methods for responding to a request to load images associated with a contact.

class ABRecord

An abstract class that defines the common properties for all Address Book records.

