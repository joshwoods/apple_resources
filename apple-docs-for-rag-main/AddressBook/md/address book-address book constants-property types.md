

- Address Book
- Address Book Constants
-  Property Types 

API Collection

# Property Types

The possible ABPropertyType types for `ABRecord` properties:

## Topics

### Constants

var kABErrorInProperty: _ABPropertyType

An invalid property was used.

var kABStringProperty: _ABPropertyType

This property is an `NSString` object.

var kABIntegerProperty: _ABPropertyType

This property is an `NSNumber` object representing an integer.

var kABRealProperty: _ABPropertyType

This property is an `NSNumber` object representing a real number.

var kABDateProperty: _ABPropertyType

This property is an `NSDate` object.

var kABArrayProperty: _ABPropertyType

This property is an `NSArray` object.

var kABDictionaryProperty: _ABPropertyType

This property is an `NSDictionary` object.

var kABDataProperty: _ABPropertyType

This property is an `NSData` object.

var kABDateComponentsProperty: _ABPropertyType

This property is an `NSDateComponents` object.

var kABMultiStringProperty: _ABPropertyType

This property is an `ABMultiValue` object containing `NSString` objects.

var kABMultiIntegerProperty: _ABPropertyType

This property is an `ABMultiValue` object containing `NSNumber` objects representing integers.

var kABMultiRealProperty: _ABPropertyType

This property is an `ABMultiValue` object containing `NSNumber` objects representing real numbers.

var kABMultiDateProperty: _ABPropertyType

This property is an `ABMultiValue` object containing `NSDate` objects.

var kABMultiArrayProperty: _ABPropertyType

This property is an `ABMultiValue` object containing `NSArray` objects.

var kABMultiDictionaryProperty: _ABPropertyType

This property is an `ABMultiValue` object containing `NSDictionary` objects.

var kABMultiDataProperty: _ABPropertyType

This property is an `ABMultiValue` object containing `NSData` objects.

var kABMultiDateComponentsProperty: _ABPropertyType

This property is an `ABMultiValue` object containing `NSDateComponents` objects.

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

Default Record Properties

Properties common to all types of records.

