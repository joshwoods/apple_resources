

- Contacts
-  Data Objects 

API Collection

# Data Objects

Access contact-related data, such as the user’s postal address and phone number.

## Topics

### Addresses

class CNPostalAddress

An immutable representation of the postal address for a contact.

class CNMutablePostalAddress

A mutable representation of the postal address for a contact.

class CNInstantMessageAddress

An immutable object representing an instant message address for the contact.

### Phone Numbers

class CNPhoneNumber

An immutable object representing a phone number for a contact.

### Groups and Containers

class CNGroup

An immutable object that represents a group of contacts.

class CNMutableGroup

A mutable object that represents a group of contacts.

class CNContainer

An immutable object that represents a collection of contacts.

### Social Profiles

class CNSocialProfile

An immutable object that represents one of the user’s social profiles.

### Related Data

class CNContactRelation

An immutable object that represents the relationship between one contact to another.

### Generic Types

class CNLabeledValue

An immutable object that combines a contact property value with a label that describes that property.

class CNContactProperty

An object that represents a property of a contact.

## See Also

### Contact data

class CNContact

An immutable object that stores information about a single contact, such as the contact’s first name, phone numbers, and addresses.

class CNMutableContact

A mutable object that stores information about a single contact, such as the contact’s first name, phone numbers, and addresses.

Contact Keys

Specify contact-related properties during fetch operations.

