

- Foundation
-  NSHashTable 

Class

# NSHashTable

A collection similar to a set, but with broader range of available memory semantics.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSHashTable where ObjectType : AnyObject
```

## Mentioned in 

NSHashTable

## Overview

The hash table is modeled after NSSet with the following differences:

- It can hold weak references to its members.

- Its members may be copied on input or may use pointer identity for equality and hashing.

- It can contain arbitrary pointers (its members are not constrained to being objects).

You can configure an NSHashTable instance to operate on arbitrary pointers and not just objects, although typically you are encouraged to use the C function API for void \* pointers. The object-based API (such as add(_:)) will not work for non-object pointers without type-casting.

Because of its options, `NSHashTable` is not a set because it can behave differently (for example, if pointer equality is specified two `isEqual:` strings will both be entered).

When configuring hash tables, note that only the options listed in NSHashTableOptions guarantee that the rest of the API will work correctly—including copying, archiving, and fast enumeration. While other NSPointerFunctions options are used for certain configurations, such as to hold arbitrary pointers, not all combinations of the options are valid. With some combinations the hash table may not work correctly, or may not even be initialized correctly.

### Subclassing Notes

`NSHashTable` is not suitable for subclassing.

## Topics

### Initialization

init(options: NSPointerFunctions.Options, capacity: Int)

Returns a hash table initialized with the given attributes.

init(pointerFunctions: NSPointerFunctions, capacity: Int)

Returns a hash table initialized with the given functions and capacity.

### Convenience Constructors

class func weakObjects() -> NSHashTable&lt;ObjectType>

Returns a new hash table for storing weak references to its contents.

init(options: NSPointerFunctions.Options)

Returns a hash table with given pointer functions options.

### Accessing Content

var anyObject: ObjectType?

One of the objects in the hash table.

var allObjects: [ObjectType]

The hash table’s members.

var setRepresentation: Set&lt;AnyHashable>

A set that contains the hash table’s members.

var count: Int

The number of elements in the hash table.

func contains(ObjectType?) -> Bool

Returns a Boolean value that indicates whether the hash table contains a given object.

func member(ObjectType?) -> ObjectType?

Determines whether the hash table contains a given object, and returns that object if it is present

func objectEnumerator() -> NSEnumerator

Returns an enumerator object that lets you access each object in the hash table.

### Manipulating Membership

func add(ObjectType?)

Adds a given object to the hash table.

func remove(ObjectType?)

Removes a given object from the hash table.

func removeAllObjects()

Removes all objects from the hash table.

### Comparing Hash Tables

func intersect(NSHashTable&lt;ObjectType>)

Removes from the receiving hash table each element that isn’t a member of another given hash table.

func intersects(NSHashTable&lt;ObjectType>) -> Bool

Returns a Boolean value that indicates whether a given hash table intersects with the receiving hash table.

func isSubset(of: NSHashTable&lt;ObjectType>) -> Bool

Returns a Boolean value that indicates whether every element in the receiving hash table is also present in another given hash table.

func isEqual(to: NSHashTable&lt;ObjectType>) -> Bool

Returns a Boolean value that indicates whether a given hash table is equal to the receiving hash table.

### Set Functions

func minus(NSHashTable&lt;ObjectType>)

Removes each element in another given hash table from the receiving hash table, if present.

func union(NSHashTable&lt;ObjectType>)

Adds each element in another given hash table to the receiving hash table, if not present.

### Accessing Pointer Functions

var pointerFunctions: NSPointerFunctions

The pointer functions for the hash table.

class NSPointerFunctions

An instance of `NSPointerFunctions` defines callout functions appropriate for managing a pointer reference held somewhere else.

### Constants

typealias NSHashTableOptions

Components in a bit-field to specify the behavior of elements in an NSHashTable object.

### Deprecated

Legacy Hash Table Implementation

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

class NSMapTable

A collection similar to a dictionary, but with a broader range of available memory semantics.

