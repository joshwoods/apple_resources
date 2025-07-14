

- Address Book
-  Address Book Constants 

API Collection

# Address Book Constants

Get the constants you use to specify Address Book information.

## Topics

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

Default Record Properties

Properties common to all types of records.

Property Types

The possible ABPropertyType types for `ABRecord` properties:

### Social Media Constants

Instant Messaging Keys

The keys used to specify the different fields in a kABInstantMessageProperty property.

Instant Messaging Services

The predefined constants are used to identify instant messaging services.

Social Profile Services

The predefined constants are used to identify social networking services.

### Errors

let ABAddressBookErrorDomain: CFString!

Error domain returning errors reported by an address book object.

Deprecated

Error Codes

Errors codes used by the Address Book framework.

### Miscellaneous

var ABMultipleValueSelection: ABPeoplePickerSelectionBehavior

The user can select multiple values.

var ABNoValueSelection: ABPeoplePickerSelectionBehavior

The user cannot select individual values.

var ABSingleValueSelection: ABPeoplePickerSelectionBehavior

The user can select a single value.

let kABAlternateBirthdayComponentsProperty: String

The components that represent a birthday in a non-Gregorian calendar.

var kABBitsInBitFieldMatch: _ABSearchComparison

Search for elements that match the bits in ABPersonFlags.

var kABContainsSubString: _ABSearchComparison

Search for elements that contain the value.

var kABContainsSubStringCaseInsensitive: _ABSearchComparison

Search for elements that contain the value,ignoring case.

var kABDefaultNameOrdering: Int32

Default name ordering (whether a person’s first name or last name is displayed first) in the Address Book application.

let kABDeletedRecords: String

Records that have been deleted.

var kABDoesNotContainSubString: _ABSearchComparison

Search for elements that do not contain the value.

var kABDoesNotContainSubStringCaseInsensitive: _ABSearchComparison

Search for elements that do not contain the value, ignoring case.

var kABEqual: _ABSearchComparison

Search for elements that are equal to the value.

var kABEqualCaseInsensitive: _ABSearchComparison

Search for elements that are equal to the value,ignoring case.

var kABFirstNameFirst: Int32

First name is displayed first in Address Book.

var kABGreaterThan: _ABSearchComparison

Search for elements that are greater than thevalue.

var kABGreaterThanOrEqual: _ABSearchComparison

Search for elements that are greater than orequal to the value.

let kABInsertedRecords: String

Records that have been inserted.

var kABLastNameFirst: Int32

Last name is displayed first in Address Book.

var kABLessThan: _ABSearchComparison

Search for elements that are less than thevalue.

var kABLessThanOrEqual: _ABSearchComparison

Search for elements that are less than or equalto the value.

var kABMultiValueInvalidIdentifier: Int32

Invalid multivalue property.

var kABNameOrderingMask: Int32

Used in conjunction with `kABDefaultNameOrdering`, `kABFirstNameFirst`, and `kABLastNameFirst` to determine name ordering.

var kABNotEqual: _ABSearchComparison

Search for elements that are not equal to thevalue.

var kABNotEqualCaseInsensitive: _ABSearchComparison

Search for elements that are not equal to the value, ignoring case.

var kABNotWithinIntervalAroundToday: _ABSearchComparison

Search for elements that are *not* within a time interval (in seconds) forward or backward from today.

var kABNotWithinIntervalAroundTodayYearless: _ABSearchComparison

Search for elements that are *not* within a time interval (in seconds) forward or backward from this day in any year.

var kABNotWithinIntervalFromToday: _ABSearchComparison

Search for elements that are *not* within a time interval (in seconds) forward from today.

var kABNotWithinIntervalFromTodayYearless: _ABSearchComparison

Search for elements that are *not* within a time interval (in seconds) forward from this day in any year.

let kABOrganizationPhoneticProperty: String

The phonetic representation of an organization name.

var kABPrefixMatch: _ABSearchComparison

Search for elements that begin with the value.

var kABPrefixMatchCaseInsensitive: _ABSearchComparison

Search for elements that begin with the value, ignoring case.

var kABPropertyInvalidID: Int32

Indicates an invalid value for a property ID.

var kABRecordInvalidID: Int32

Records with this ID have not been saved to the Address Book database.

var kABSearchAnd: _ABSearchConjunction

Join the search elements together with theAND operand.

var kABSearchOr: _ABSearchConjunction

Join the search elements together with theOR operand.

var kABShowAsCompany: Int32

Record is displayed as a company.

var kABShowAsMask: Int32

Used in conjunction with `kABShowAsPerson` and `kABShowAsCompany` to determine record configuration.

var kABShowAsPerson: Int32

Record is displayed as a person.

var kABShowAsResource: Int32

Record is displayed as a resource.

var kABShowAsRoom: Int32

Record is displayed as a room.

let kABSocialProfileServiceTencentWeibo: String

The user’s Tencent Weibo profile identifier.

let kABSocialProfileServiceYelp: String

The user’s Yelp profile identifier.

var kABSourceTypeSearchableMask: Int32

Indicates that a source is searchable.

var kABSuffixMatch: _ABSearchComparison

Search for elements that end with the value.

var kABSuffixMatchCaseInsensitive: _ABSearchComparison

Search for elements that end with the value, ignoring case.

let kABUpdatedRecords: String

Records that have been updated.

var kABWithinIntervalAroundToday: _ABSearchComparison

Search for elements that are within a time interval (in seconds) forward or backward from today.

var kABWithinIntervalAroundTodayYearless: _ABSearchComparison

Search for elements that are within a time interval (in seconds) forward or backward from this day in any year.

var kABWithinIntervalFromToday: _ABSearchComparison

Search for elements that are within a time interval (in seconds) forward from today.

var kABWithinIntervalFromTodayYearless: _ABSearchComparison

Search for elements that are within a time interval (in seconds) forward from this day in any year.

### Deprecated

let kABPersonAddressCityKey: CFString!

City.

Deprecated

let kABPersonAddressCountryCodeKey: CFString!

Country code. The value is an ISO country code.

Deprecated

let kABPersonAddressCountryKey: CFString!

Country or region.

Deprecated

let kABPersonAddressProperty: ABPropertyID

Identifier for the address multivalue property.

Deprecated

let kABPersonAddressStateKey: CFString!

State.

Deprecated

let kABPersonAddressStreetKey: CFString!

Street.

Deprecated

let kABPersonAddressZIPKey: CFString!

Zip code.

Deprecated

let kABPersonAlternateBirthdayCalendarIdentifierKey: CFString!

The associated value is a string representing the calendar identifier for a CFCalendar.

Deprecated

let kABPersonAlternateBirthdayDayKey: CFString!

The associated value is a CFNumber of type CFNumberType.nsIntegerType whose value is the day for the birthday.

Deprecated

let kABPersonAlternateBirthdayEraKey: CFString!

The associated value is a CFNumber of type CFNumberType.nsIntegerType whose value is the era for the birthday.

Deprecated

let kABPersonAlternateBirthdayIsLeapMonthKey: CFString!

The associated value is a CFNumber of type CFNumberType.charType.

Deprecated

let kABPersonAlternateBirthdayMonthKey: CFString!

The associated value is a CFNumber of type CFNumberType.nsIntegerType whose value is the month for the birthday.

Deprecated

let kABPersonAlternateBirthdayProperty: ABPropertyID

The associated value is a kABDictionaryPropertyType with keys specified by the other constants listed here.

Deprecated

let kABPersonAlternateBirthdayYearKey: CFString!

The associated value is a CFNumber of type CFNumberType.nsIntegerType whose value is the year for the birthday.

Deprecated

let kABPersonAnniversaryLabel: CFString!

Birthdate.

Deprecated

let kABPersonAssistantLabel: CFString!

Assistant.

Deprecated

let kABPersonBirthdayProperty: ABPropertyID

Birthday. Type: kABDateTimePropertyType.

Deprecated

let kABPersonBrotherLabel: CFString!

Brother.

Deprecated

let kABPersonChildLabel: CFString!

Child.

Deprecated

let kABPersonCreationDateProperty: ABPropertyID

Creation date. Type: kABDateTimePropertyType.

Deprecated

let kABPersonDateProperty: ABPropertyID

Identifier for the dates multivalue property.

Deprecated

let kABPersonDepartmentProperty: ABPropertyID

Department. Type: kABStringPropertyType.

Deprecated

let kABPersonEmailProperty: ABPropertyID

Email address. Type: kABMultiStringPropertyType.

Deprecated

let kABPersonFatherLabel: CFString!

Father.

Deprecated

let kABPersonFirstNamePhoneticProperty: ABPropertyID

First name phonetic. Type: kABStringPropertyType.

Deprecated

let kABPersonFirstNameProperty: ABPropertyID

First name. Type: kABStringPropertyType.

Deprecated

let kABPersonFriendLabel: CFString!

Friend.

Deprecated

let kABPersonHomePageLabel: CFString!

Home page.

Deprecated

var kABPersonImageFormatOriginalSize: ABPersonImageFormat

The image at its original size and shape.

var kABPersonImageFormatThumbnail: ABPersonImageFormat

The small square thumbnail.

let kABPersonInstantMessageProperty: ABPropertyID

Identifier for the instant message multivalue property.

Deprecated

let kABPersonInstantMessageServiceAIM: CFString!

AIM instant message service.

Deprecated

let kABPersonInstantMessageServiceFacebook: CFString!

Facebook instant message service.

Deprecated

let kABPersonInstantMessageServiceGaduGadu: CFString!

Gadu-Gadu instant message service.

Deprecated

let kABPersonInstantMessageServiceGoogleTalk: CFString!

Google Talk instant message service.

Deprecated

let kABPersonInstantMessageServiceICQ: CFString!

ICQ instant message service.

Deprecated

let kABPersonInstantMessageServiceJabber: CFString!

Jabber instant message service.

Deprecated

let kABPersonInstantMessageServiceKey: CFString!

Instant message service.

Deprecated

let kABPersonInstantMessageServiceMSN: CFString!

MSN instant message service.

Deprecated

let kABPersonInstantMessageServiceQQ: CFString!

QQ instant message service.

Deprecated

let kABPersonInstantMessageServiceSkype: CFString!

Skype instant message service.

Deprecated

let kABPersonInstantMessageServiceYahoo: CFString!

Yahoo instant message service.

Deprecated

let kABPersonInstantMessageUsernameKey: CFString!

Instant message service username.

Deprecated

let kABPersonJobTitleProperty: ABPropertyID

Job title. Type: kABStringPropertyType.

Deprecated

let kABPersonKindOrganization: CFNumber!

Identifies an organization.

Deprecated

let kABPersonKindPerson: CFNumber!

Identifies a person.

Deprecated

let kABPersonKindProperty: ABPropertyID

Identifier for the type property.

Deprecated

let kABPersonLastNamePhoneticProperty: ABPropertyID

Last name phonetic. Type: kABStringPropertyType.

Deprecated

let kABPersonLastNameProperty: ABPropertyID

Last name. Type: kABStringPropertyType.

Deprecated

let kABPersonManagerLabel: CFString!

Manager.

Deprecated

let kABPersonMiddleNamePhoneticProperty: ABPropertyID

Middle name phonetic. Type: kABStringPropertyType.

Deprecated

let kABPersonMiddleNameProperty: ABPropertyID

Middle name. Type: kABStringPropertyType.

Deprecated

let kABPersonModificationDateProperty: ABPropertyID

Modification date. Type: kABDateTimePropertyType.

Deprecated

let kABPersonMotherLabel: CFString!

Mother.

Deprecated

let kABPersonNicknameProperty: ABPropertyID

Nickname. Type: kABStringPropertyType.

Deprecated

let kABPersonNoteProperty: ABPropertyID

Note. Type: kABStringPropertyType.

Deprecated

let kABPersonOrganizationProperty: ABPropertyID

Organization name. Type: kABStringPropertyType.

Deprecated

let kABPersonParentLabel: CFString!

Parent.

Deprecated

let kABPersonPartnerLabel: CFString!

Partner.

Deprecated

let kABPersonPhoneHomeFAXLabel: CFString!

Home fax number.

Deprecated

let kABPersonPhoneIPhoneLabel: CFString!

iPhone number.

Deprecated

let kABPersonPhoneMainLabel: CFString!

Main phone number.

Deprecated

let kABPersonPhoneMobileLabel: CFString!

Mobile phone number.

Deprecated

let kABPersonPhoneOtherFAXLabel: CFString!

Other fax number.

Deprecated

let kABPersonPhonePagerLabel: CFString!

Pager phone number.

Deprecated

let kABPersonPhoneProperty: ABPropertyID

Identifier for the phone number multivalue property.

Deprecated

let kABPersonPhoneWorkFAXLabel: CFString!

Work fax number.

Deprecated

let kABPersonPrefixProperty: ABPropertyID

Prefix (“Sir,” “Duke,” “General”). Type: kABStringPropertyType.

Deprecated

let kABPersonRelatedNamesProperty: ABPropertyID

Identifier for the related name multivalue property.

Deprecated

let kABPersonSisterLabel: CFString!

Sister.

Deprecated

let kABPersonSocialProfileProperty: ABPropertyID

Identifier for the social profile property.

Deprecated

let kABPersonSocialProfileServiceFacebook: CFString!

Facebook social profile service.

Deprecated

let kABPersonSocialProfileServiceFlickr: CFString!

Flickr social profile service.

Deprecated

let kABPersonSocialProfileServiceGameCenter: CFString!

Game Center social profile service.

Deprecated

let kABPersonSocialProfileServiceKey: CFString!

Social profile service.

Deprecated

let kABPersonSocialProfileServiceLinkedIn: CFString!

LinkedIn social profile service.

Deprecated

let kABPersonSocialProfileServiceMyspace: CFString!

Myspace social profile service.

Deprecated

let kABPersonSocialProfileServiceSinaWeibo: CFString!

Sina Weibo social profile service.

Deprecated

let kABPersonSocialProfileServiceTwitter: CFString!

Twitter social profile service.

Deprecated

let kABPersonSocialProfileURLKey: CFString!

Social profile URL.

Deprecated

let kABPersonSocialProfileUserIdentifierKey: CFString!

Social profile user identifier.

Deprecated

let kABPersonSocialProfileUsernameKey: CFString!

Social profile username.

Deprecated

let kABPersonSpouseLabel: CFString!

Spouse.

Deprecated

let kABPersonSuffixProperty: ABPropertyID

Suffix (“Jr.,” “Sr.,” “III”). Type: kABStringPropertyType.

Deprecated

let kABPersonURLProperty: ABPropertyID

Identifier for the URL multivalue property.

Deprecated

let kABSourceNameProperty: ABPropertyID

The name of the source. Type: kABStringPropertyType.

Deprecated

let kABSourceTypeProperty: ABPropertyID

The type of the source.

Deprecated

## See Also

### C Interfaces

C Types

Identify the C types that correspond to Address Book objects.

AddressBook Functions

Find the C functions and function-like macros you use to manipulate Address Book data.

AddressBook Enumerations

Get the enumerations you use to specify Address Book information.

AddressBook Data Types

Get the data types you use to specify Address Book information.

