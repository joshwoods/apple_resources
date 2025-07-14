

- Address Book
- Address Book Constants
-  Address Keys 

API Collection

# Address Keys

The keys used to specify the different fields in a `kABAddressProperty`.

## Overview

Neither developers nor users can add more keys.

## Topics

### Constants

let kABAddressStreetKey: String

Street.

let kABAddressCityKey: String

City.

let kABAddressStateKey: String

State.

let kABAddressZIPKey: String

Zip.

let kABAddressCountryKey: String

Country name.

let kABAddressCountryCodeKey: String

Country, identified by ISO country code. For a list of these codes, see ABPerson.

## See Also

### Data Type Constants

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

Default Record Properties

Properties common to all types of records.

Property Types

The possible ABPropertyType types for `ABRecord` properties:

