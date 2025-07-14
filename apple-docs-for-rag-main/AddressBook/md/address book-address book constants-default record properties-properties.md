

- Address Book
- Address Book Constants
-  Default Record Properties 

API Collection

# Default Record Properties

Properties common to all types of records.

## Topics

### Constants

let kABUIDProperty: String

The unique ID for this record. It’s guaranteed never to change, no matter how much the record changes. If you need to store a reference to a record, use this value. Type: kABStringProperty.

let kABCreationDateProperty: String

The date when the record was first saved. Type: kABDateProperty.

let kABModificationDateProperty: String

The date when the record was last saved. Type: kABDateProperty.

## See Also

### Data Type Constants

Address Keys

The keys used to specify the different fields in a `kABAddressProperty`.

Default Person Properties

The properties that a person record contains by default.

Default Group Properties

The properties that a group record contains by default. Developers can add their own properties with the `ABGroup` method addPropertiesAndTypes(_:)

Default Multivalue List Labels

The default labels contained in the Address Book database for specifying different values in a multivalue list. Users can also add their own labels.

Generic Multivalue List Labels

The generic labels contained in the Address Book database for specifying different values in a multivalue list.

Multivalue Property

A multivalue property type.

Property Types

The possible ABPropertyType types for `ABRecord` properties:

