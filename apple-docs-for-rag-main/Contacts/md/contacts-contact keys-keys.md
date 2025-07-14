

- Contacts
-  Contact Keys 

API Collection

# Contact Keys

Specify contact-related properties during fetch operations.

## Topics

### Contact Identification

let CNContactIdentifierKey: String

The contact’s unique identifier.

let CNContactTypeKey: String

The type of contact.

let CNContactPropertyAttribute: String

The contact’s name component property key.

### Name

let CNContactNamePrefixKey: String

The prefix for the contact’s name.

let CNContactGivenNameKey: String

The contact’s given name.

let CNContactMiddleNameKey: String

The contact’s middle name.

let CNContactFamilyNameKey: String

The contact’s family name.

let CNContactPreviousFamilyNameKey: String

The contact’s previous family name.

let CNContactNameSuffixKey: String

The contact’s name suffix.

let CNContactNicknameKey: String

The contact’s nickname.

let CNContactPhoneticGivenNameKey: String

The phonetic spelling of the contact’s given name.

let CNContactPhoneticMiddleNameKey: String

The phonetic spelling of the contact’s middle name.

let CNContactPhoneticFamilyNameKey: String

The phonetic spelling of the contact’s family name.

### Work

let CNContactJobTitleKey: String

The contact’s job title.

let CNContactDepartmentNameKey: String

The contact’s department name.

let CNContactOrganizationNameKey: String

The contact’s organization name.

let CNContactPhoneticOrganizationNameKey: String

The phonetic spelling of the contact’s organization name.

### Addresses

let CNContactPostalAddressesKey: String

The postal addresses of the contact.

let CNContactEmailAddressesKey: String

The email addresses of the contact.

let CNContactUrlAddressesKey: String

The URL addresses of the contact.

let CNContactInstantMessageAddressesKey: String

The instant message addresses of the contact.

### Phone

let CNContactPhoneNumbersKey: String

A phone numbers of a contact.

### Social Profiles

let CNContactSocialProfilesKey: String

A social profiles of a contact.

### Birthday

let CNContactBirthdayKey: String

The birthday of a contact.

let CNContactNonGregorianBirthdayKey: String

The non-Gregorian birthday of the contact.

let CNContactDatesKey: String

Dates associated with a contact.

### Notes

let CNContactNoteKey: String

A note associated with a contact.

com.apple.developer.contacts.notes

A Boolean value that indicates whether the app may access the notes in contact entries.

### Images

let CNContactImageDataKey: String

Image data for a contact.

let CNContactThumbnailImageDataKey: String

Thumbnail data for a contact.

let CNContactImageDataAvailableKey: String

Image data availability for a contact.

### Relationships

let CNContactRelationsKey: String

The relationships of the contact.

### Groups and Containers

let CNGroupNameKey: String

The name of the group.

let CNGroupIdentifierKey: String

The identifier of the group.

let CNContainerNameKey: String

The name of the container.

let CNContainerTypeKey: String

The type of the container.

### Instant Messaging Keys

let CNInstantMessageAddressServiceKey: String

Instant message address service key.

let CNInstantMessageAddressUsernameKey: String

Instant message address username key.

### Social Profile Keys

let CNSocialProfileServiceKey: String

The social profile service.

let CNSocialProfileURLStringKey: String

The social profile URL.

let CNSocialProfileUsernameKey: String

The social profile user name.

let CNSocialProfileUserIdentifierKey: String

The social profile user identifier.

### Key Descriptors

protocol CNKeyDescriptor

This protocol is reserved for Contacts framework usage.

## See Also

### Contact data

class CNContact

An immutable object that stores information about a single contact, such as the contact’s first name, phone numbers, and addresses.

class CNMutableContact

A mutable object that stores information about a single contact, such as the contact’s first name, phone numbers, and addresses.

Data Objects

Access contact-related data, such as the user’s postal address and phone number.

