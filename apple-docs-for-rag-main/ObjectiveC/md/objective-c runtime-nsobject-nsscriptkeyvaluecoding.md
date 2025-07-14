

- Objective-C Runtime
- NSObject
-  NSScriptKeyValueCoding 

API Collection

# NSScriptKeyValueCoding

A collection of methods that provide additional capabilities for working with key-value coding.

## Overview

Cocoa scripting takes advantage of key-value coding to get and set information in scriptable objects. The methods in this category provide additional capabilities for working with key-value coding, including getting and setting key values by index in multi-value keys and coercing (or converting) a key value. Additional methods allow the implementer of a scriptable container class to provide fast access to elements that are being referenced by name and unique ID.

Because Cocoa scripting invokes setValue(_:forKey:) and mutableArrayValue(forKey:), changes to model objects made by AppleScript scripts are observable using automatic key-value observing.

Note

In OS X 10.3 and earlier, Cocoa scripting did not invoke setValue(_:forKey:) or mutableArrayValue(forKey:), so automatic key-value observing notification was not always done for model object changes caused by scripts. Starting in macOS 10.4, for backward binary compatibility, if it is overridden, Cocoa invokes the now-deprecated method takeValue(_:forKey:) instead of setValue(_:forKey:).

## Topics

### Indexed access

func insertValue(Any, at: Int, inPropertyWithKey: String)

Inserts an object at the specified index in the collection specified by the passed key.

func removeValue(at: Int, fromPropertyWithKey: String)

Removes the object at the specified index from the collection specified by the passed key.

func replaceValue(at: Int, inPropertyWithKey: String, withValue: Any)

Replaces the object at the specified index in the collection specified by the passed key.

func value(at: Int, inPropertyWithKey: String) -> Any?

Retrieves an indexed object from the collection specified by the passed key.

### Access by name, key, or ID

func insertValue(Any, inPropertyWithKey: String)

Inserts an object in the collection specified by the passed key.

func value(withName: String, inPropertyWithKey: String) -> Any?

Retrieves a named object from the collection specified by the passed key.

func value(withUniqueID: Any, inPropertyWithKey: String) -> Any?

Retrieves an object by ID from the collection specified by the passed key.

### Coercion

func coerceValue(Any?, forKey: String) -> Any?

Uses type info from the class description and `NSScriptCoercionHandler` to attempt to convert `value` for `key` to the proper type, if necessary.

### Constants

NSScriptKeyValueCoding Exception Names

Exceptions raised by key-value coding methods.

## See Also

### Related Documentation

Cocoa Scripting Guide

Key-Value Coding Programming Guide

### Key-Value Coding

NSKeyValueBindingCreation

A set of methods that you can use to create and remove bindings between view objects and controllers, or between controllers and model objects.

NSKeyValueCoding

A mechanism by which you can access the properties of an object indirectly by name or key.

NSScriptKeyValueCoding Exception Names

Exceptions raised by key-value coding methods.

