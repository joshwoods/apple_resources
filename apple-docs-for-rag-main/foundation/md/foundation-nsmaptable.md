

- Foundation
-  NSMapTable 

Class

# NSMapTable

A collection similar to a dictionary, but with a broader range of available memory semantics.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSMapTable where KeyType : AnyObject, ObjectType : AnyObject
```

## Mentioned in 

NSMapTable

## Overview

The map table is modeled after NSDictionary with the following differences:

- Keys and/or values are optionally held “weakly” such that entries are removed when one of the objects is reclaimed.

- Its keys or values may be copied on input or may use pointer identity for equality and hashing.

- It can contain arbitrary pointers (its contents are not constrained to being objects).

You can configure an NSMapTable instance to operate on arbitrary pointers and not just objects, although typically you are encouraged to use the C function API for void \* pointers. The object-based API (such as setObject(_:forKey:)) will not work for non-object pointers without type-casting.

When configuring map tables, note that only the options listed in NSMapTableOptions guarantee that the rest of the API will work correctly—including copying, archiving, and fast enumeration. While other NSPointerFunctions options are used for certain configurations, such as to hold arbitrary pointers, not all combinations of the options are valid. With some combinations the map table may not work correctly, or may not even be initialized correctly.

### Subclassing Notes

`NSMapTable` is not suitable for subclassing.

## Topics

### Creating and Initializing a Map Table

init(keyOptions: NSPointerFunctions.Options, valueOptions: NSPointerFunctions.Options, capacity: Int)

Returns a map table, initialized with the given options.

init(keyOptions: NSPointerFunctions.Options, valueOptions: NSPointerFunctions.Options)

Returns a new map table, initialized with the given options

init(keyPointerFunctions: NSPointerFunctions, valuePointerFunctions: NSPointerFunctions, capacity: Int)

Returns a map table, initialized with the given functions.

class func strongToStrongObjects() -> NSMapTable&lt;KeyType, ObjectType>

Returns a new map table object which has strong references to the keys and values.

class func weakToStrongObjects() -> NSMapTable&lt;KeyType, ObjectType>

Returns a new map table object which has weak references to the keys and strong references to the values.

class func strongToWeakObjects() -> NSMapTable&lt;KeyType, ObjectType>

Returns a new map table object which has strong references to the keys and weak references to the values.

class func weakToWeakObjects() -> NSMapTable&lt;KeyType, ObjectType>

Returns a new map table object which has weak references to the keys and values.

typealias NSMapTableOptions

Constants used as components in a bitfield to specify the behavior of elements (keys and values) in an `NSMapTable` object.

### Accessing Content

func object(forKey: KeyType?) -> ObjectType?

Returns a the value associated with a given key.

func keyEnumerator() -> NSEnumerator

Returns an enumerator object that lets you access each key in the map table.

func objectEnumerator() -> NSEnumerator?

Returns an enumerator object that lets you access each value in the map table.

var count: Int

The number of key-value pairs in the map table.

### Manipulating Content

func setObject(ObjectType?, forKey: KeyType?)

Adds a given key-value pair to the map table.

func removeObject(forKey: KeyType?)

Removes a given key and its associated value from the map table.

func removeAllObjects()

Empties the map table of its entries.

### Creating a Dictionary Representation

func dictionaryRepresentation() -> [AnyHashable : ObjectType]

Returns a dictionary representation of the map table.

### Accessing Pointer Functions

var keyPointerFunctions: NSPointerFunctions

The pointer functions the map table uses to manage keys.

var valuePointerFunctions: NSPointerFunctions

The pointer functions the map table uses to manage values.

class NSPointerFunctions

An instance of `NSPointerFunctions` defines callout functions appropriate for managing a pointer reference held somewhere else.

### Deprecated

Legacy Map Table Implementation

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSFastEnumeration
- NSObjectProtocol
- NSSecureCoding

## See Also

### Pointer Collections

class NSPointerArray

A collection similar to an array, but with a broader range of available memory semantics.

class NSHashTable

A collection similar to a set, but with broader range of available memory semantics.

