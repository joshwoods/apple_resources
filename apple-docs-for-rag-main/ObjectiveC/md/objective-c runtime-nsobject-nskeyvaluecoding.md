

- Objective-C Runtime
- NSObject
-  NSKeyValueCoding 

API Collection

# NSKeyValueCoding

A mechanism by which you can access the properties of an object indirectly by name or key.

## Overview

The basic methods for accessing an object’s values are setValue(_:forKey:), which sets the value for the property identified by the specified key, and value(forKey:), which returns the value for the property identified by the specified key. Thus, all of an object’s properties can be accessed in a consistent manner.

The default implementation relies on the accessor methods normally implemented by objects (or to access instance variables directly if need be).

## Topics

### Getting Values

func value(forKey: String) -> Any?

Returns the value for the property identified by a given key.

func value(forKeyPath: String) -> Any?

Returns the value for the derived property identified by a given key path.

func dictionaryWithValues(forKeys: [String]) -> [String : Any]

Returns a dictionary containing the property values identified by each of the keys in a given array.

func value(forUndefinedKey: String) -> Any?

Invoked by value(forKey:) when it finds no property corresponding to a given key.

func mutableArrayValue(forKey: String) -> NSMutableArray

Returns a mutable array proxy that provides read-write access to an ordered to-many relationship specified by a given key.

func mutableArrayValue(forKeyPath: String) -> NSMutableArray

Returns a mutable array that provides read-write access to the ordered to-many relationship specified by a given key path.

func mutableSetValue(forKey: String) -> NSMutableSet

Returns a mutable set proxy that provides read-write access to the unordered to-many relationship specified by a given key.

func mutableSetValue(forKeyPath: String) -> NSMutableSet

Returns a mutable set that provides read-write access to the unordered to-many relationship specified by a given key path.

func mutableOrderedSetValue(forKey: String) -> NSMutableOrderedSet

Returns a mutable ordered set that provides read-write access to the uniquing ordered to-many relationship specified by a given key.

func mutableOrderedSetValue(forKeyPath: String) -> NSMutableOrderedSet

Returns a mutable ordered set that provides read-write access to the uniquing ordered to-many relationship specified by a given key path.

### Setting Values

func setValue(Any?, forKeyPath: String)

Sets the value for the property identified by a given key path to a given value.

func setValuesForKeys([String : Any])

Sets properties of the receiver with values from a given dictionary, using its keys to identify the properties.

func setNilValueForKey(String)

Invoked by setValue(_:forKey:) when it’s given a `nil` value for a scalar value (such as an `int` or `float`).

func setValue(Any?, forKey: String)

Sets the property of the receiver specified by a given key to a given value.

func setValue(Any?, forUndefinedKey: String)

Invoked by setValue(_:forKey:) when it finds no property for a given key.

### Changing Default Behavior

class var accessInstanceVariablesDirectly: Bool

Returns a Boolean value that indicates whether the key-value coding methods should access the corresponding instance variable directly on finding no accessor method for a property.

### Validation

func validateValue(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>, forKey: String) throws

Indicates whether the value specified by a given pointer is valid, or can be made valid, for the property identified by a given key.

func validateValue(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>, forKeyPath: String) throws

Indicates whether the value specified by a given pointer is not valid for a given key path relative to the receiver.

### Deprecated Methods

class func useStoredAccessor() -> Bool

Returns `true` if the stored value methods storedValue(forKey:) and takeStoredValue(_:forKey:) should use private accessor methods in preference to public accessors.

Deprecated

func handleQuery(withUnboundKey: String) -> Any?

Invoked by value(forKey:) when it finds no property corresponding to `key`.

Deprecated

func handleTakeValue(Any?, forUnboundKey: String)

Invoked by takeValue(_:forKey:) when it finds no property binding for `key`.

Deprecated

func storedValue(forKey: String) -> Any?

Returns the property identified by a given key.

Deprecated

func takeStoredValue(Any?, forKey: String)

Sets the value of the property identified by a given key.

Deprecated

func takeValues(from: [AnyHashable : Any])

Sets properties of the receiver with values from a given dictionary, using its keys to identify the properties

Deprecated

func takeValue(Any?, forKeyPath: String)

Sets the value for the property identified by `keyPath` to `value`.

Deprecated

func takeValue(Any?, forKey: String)

Sets the value for the property identified by `key` to `value`.

Deprecated

func unableToSetNil(forKey: String)

Invoked if `key` is represented by a scalar attribute.

Deprecated

func values(forKeys: [Any]) -> [AnyHashable : Any]

Returns a dictionary containing as keys the property names in `keys`, with corresponding values being the corresponding property values.

Deprecated

### Constants

Key Value Coding Exception Names

This constant defines the name of an exception raised when a key value coding operation fails.

NSUndefinedKeyException userInfo Keys

These constants are keys into an `NSUndefinedKeyException` `userInfo` dictionary

var NSKeyValueValidationError: Int

A key-value coding validation error.

## See Also

### Related Documentation

Key-Value Coding Programming Guide

### Key-Value Coding

NSKeyValueBindingCreation

A set of methods that you can use to create and remove bindings between view objects and controllers, or between controllers and model objects.

NSScriptKeyValueCoding

A collection of methods that provide additional capabilities for working with key-value coding.

NSScriptKeyValueCoding Exception Names

Exceptions raised by key-value coding methods.

