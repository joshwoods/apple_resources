

- Address Book
- Address Book Constants
-  Generic Multivalue List Labels 

API Collection

# Generic Multivalue List Labels

The generic labels contained in the Address Book database for specifying different values in a multivalue list.

## Overview

These labels are especially useful if there is no default label for a property. Users can also add their own labels.

## Topics

### Constants

let kABWorkLabel: CFString!

All Work labels match this label.

Deprecated

let kABHomeLabel: CFString!

All Home labels match this label.

Deprecated

let kABOtherLabel: CFString!

All labels other than Home or Work labels match this label.

Deprecated

let kABMobileMeLabel: String

MobileMe instant messenger or email values.

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

Multivalue Property

A multivalue property type.

Default Record Properties

Properties common to all types of records.

Property Types

The possible ABPropertyType types for `ABRecord` properties:

