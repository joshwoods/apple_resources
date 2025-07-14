

- Contacts
-  CNMutableContact 

Class

# CNMutableContact

A mutable object that stores information about a single contact, such as the contact’s first name, phone numbers, and addresses.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
class CNMutableContact
```

## Overview

`CNMutableContact` objects are not a thread-safe class. To access the contact information in a thread-safe manner, use a CNContact object instead.

You may modify only those properties whose values you fetched from the contacts database. When fetching a contact, you specify which properties you want to retrieve from the database. The contact store then populates the properties of a CNContact object with those values. After creating a mutable copy of that object, you can modify only those properties for which a value exists. If you attempt to access a property that is not available, the `CNMutableContact` object throws a CNContactPropertyNotFetchedExceptionName exception.

To remove the value for a property, set string and array properties to empty, and set all other properties to `nil`.

## Topics

### Setting the Identity of the Contact

var contactType: CNContactType

An enum identifying the contact type.

### Setting Name Information

var namePrefix: String

The name prefix of the contact.

var givenName: String

The given name of the contact.

var middleName: String

The middle name of the contact.

var familyName: String

The family name of the contact.

var previousFamilyName: String

The previous family name of the contact.

var nameSuffix: String

The name suffix of the contact.

var nickname: String

The nickname of the contact.

var phoneticGivenName: String

The phonetic given name of the contact.

var phoneticMiddleName: String

The phonetic middle name of the contact.

var phoneticFamilyName: String

The phonetic family name of the contact.

### Setting Work Information

var jobTitle: String

The contact’s job title.

var departmentName: String

The name of the department associated with the contact.

var organizationName: String

The name of the organization associated with the contact.

var phoneticOrganizationName: String

The phonetic name of the organization associated with the contact.

### Setting Addresses

var postalAddresses: [CNLabeledValue&lt;CNPostalAddress>]

An array of labeled postal addresses for a contact.

var emailAddresses: [CNLabeledValue&lt;NSString>]

An array of labeled email addresses for the contact.

var urlAddresses: [CNLabeledValue&lt;NSString>]

An array of labeled URL addresses for a contact.

### Setting Phone Information

var phoneNumbers: [CNLabeledValue&lt;CNPhoneNumber>]

An array of labeled phone numbers for a contact.

### Setting Social Profiles

var socialProfiles: [CNLabeledValue&lt;CNSocialProfile>]

An array of labeled social profiles for a contact.

### Setting Birthday Information

var dates: [CNLabeledValue&lt;NSDateComponents>]

An array containing labeled Gregorian dates.

var nonGregorianBirthday: DateComponents?

A date component for the non-Gregorian birthday of the contact.

var birthday: DateComponents?

A date component for the Gregorian birthday of the contact.

### Setting Notes

var note: String

A string containing notes for the contact.

### Setting Images

var imageData: Data?

The profile picture of a contact.

### Relating Other Information to the Contact

var contactRelations: [CNLabeledValue&lt;CNContactRelation>]

An array of labeled contact relations for the contact.

var instantMessageAddresses: [CNLabeledValue&lt;CNInstantMessageAddress>]

An array of labeled IM addresses for the contact.

### Instance Properties

var id: UUID

## Relationships

### Inherits From

- CNContact

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- Identifiable
- NSCoding
- NSCopying
- NSItemProviderReading
- NSItemProviderWriting
- NSMutableCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Contact data

class CNContact

An immutable object that stores information about a single contact, such as the contact’s first name, phone numbers, and addresses.

Data Objects

Access contact-related data, such as the user’s postal address and phone number.

Contact Keys

Specify contact-related properties during fetch operations.

