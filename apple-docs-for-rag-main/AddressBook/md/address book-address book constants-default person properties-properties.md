

- Address Book
- Address Book Constants
-  Default Person Properties 

API Collection

# Default Person Properties

The properties that a person record contains by default.

## Overview

You can add your own properties with the `ABPerson` method addPropertiesAndTypes(_:).

## Topics

### Constants

let kABFirstNameProperty: String

First name. Type: kABStringProperty.

let kABLastNameProperty: String

Last name. Type: kABStringProperty.

let kABFirstNamePhoneticProperty: String

Phonetic representation of the first name. Type: kABStringProperty.

let kABLastNamePhoneticProperty: String

Phonetic representation of the last name. Type: kABStringProperty.

let kABNicknameProperty: String

Nickname. Type: kABStringProperty.

let kABMaidenNameProperty: String

Maiden name. Type: kABStringProperty.

let kABBirthdayProperty: String

Birth date. Type: kABDateProperty.

let kABBirthdayComponentsProperty: String

Birth date as date components. Type: kABDateComponentsProperty.

let kABOrganizationProperty: String

Company name. Type: kABStringProperty.

let kABJobTitleProperty: String

Job title. Type: kABStringProperty.

let kABHomePageProperty: String

Home web page. Type: kABStringProperty.

Deprecated

let kABURLsProperty: String

Web pages. Type: kABMultiStringProperty.

let kABCalendarURIsProperty: String

Calendar URIs. Type: kABMultiStringProperty.

let kABEmailProperty: String

Email addresses. Type: kABMultiStringProperty.

let kABAddressProperty: String

Street addresses. Type: kABMultiDictionaryProperty.

let kABOtherDatesProperty: String

Dates associated with a person. Type: kABMultiDateProperty.

let kABOtherDateComponentsProperty: String

Dates associated with a person, as date components. Type: kABMultiDateComponentsProperty.

let kABRelatedNamesProperty: String

Names of people related to a person.

let kABDepartmentProperty: String

Department name. Type: kABStringProperty.

let kABPersonFlags: String

Property that specifies the name ordering and configuration of a record in the Address Book application.

let kABPhoneProperty: String

Generic phone number.

let kABInstantMessageProperty: String

Instant messaging ID.

let kABNoteProperty: String

Notes. Type: kABStringProperty.

let kABSocialProfileProperty: String

Social network profile.

let kABMiddleNameProperty: String

Middle name. Type: kABStringProperty.

let kABMiddleNamePhoneticProperty: String

Phonetic representation of the middle name. Type: kABStringProperty.

let kABTitleProperty: String

Title, such as “Mr.,” “Mrs.,” “General,” “Cardinal,” or “Lord.” Type: kABStringProperty.

let kABSuffixProperty: String

Suffix, such as “Sr.,” “Jr.,” “III.,” or “Esq.” Type: kABStringProperty.

## See Also

### Data Type Constants

Address Keys

The keys used to specify the different fields in a `kABAddressProperty`.

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

