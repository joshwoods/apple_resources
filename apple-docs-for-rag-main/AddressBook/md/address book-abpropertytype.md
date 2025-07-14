

- Address Book
-  ABPropertyType 

Type Alias

# ABPropertyType

These are the possible types of ABRecord properties.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS

**iOS, iPadOS, Mac Catalyst**

``` source
typealias ABPropertyType = UInt32
```

**macOS**

``` source
typealias ABPropertyType = CFIndex
```

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

## See Also

### Miscellaneous

typealias ABSearchComparison

Constants used to specify the type of comparison beingmade.

typealias ABSearchConjunction

Constants used to create compound search elements.

