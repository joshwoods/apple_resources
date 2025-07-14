

- Kernel
- IOKit Fundamentals
- Data Types
-  OSDictionary 

Class

# OSDictionary

OSDictionary provides an associative store using strings for keys.

macOS 10.0+

``` source
class OSDictionary : OSCollection
```

## Overview

OSDictionary is a container for Libkern C++ objects (those derived from OSMetaClassBase, in particular OSObject). Storage and access are associative, based on string-valued keys (C string, `OSString`, or OSSymbol). When adding an object to an OSDictionary, you provide a string identifier, which can then used to retrieve that object or remove it from the dictionary. Setting an object with a key that already has an associated object replaces the original object.

You must generally cast retrieved objects from OSObject to the desired class using OSDynamicCast. This macro returns the object cast to the desired class, or `NULL` if the object isn't derived from that class.

When iterating an OSDictionary using OSCollectionIterator, the objects returned from getNextObject are dictionary keys (not the object values for those keys). You can use the keys to retrieve their associated object values.

As with all Libkern collection classes, OSDictionary retains keys and objects added to it, and releases keys and objects removed from it (or replaced). An OSDictionary also grows as necessary to accommodate new key/value pairs, *unlike* Core Foundation collections (it does not, however, shrink).

**Note:** OSDictionary currently uses a linear search algorithm, and is not designed for high-performance access of many values. It is intended as a simple associative-storage mechanism only.

**Use Restrictions**

With very few exceptions in the I/O Kit, all Libkern-based C++ classes, functions, and macros are **unsafe** to use in a primary interrupt context. Consult the I/O Kit documentation related to primary interrupts for more information.

OSDictionary provides no concurrency protection; it's up to the usage context to provide any protection necessary. Some portions of the I/O Kit, such as IORegistryEntry, handle synchronization via defined member functions for setting properties.

## Topics

### Miscellaneous

copyCollection

Creates a deep copy of the dictionary and its child collections.

ensureCapacity

Ensures the dictionary has enough space to store the requested number of key/object pairs.

flushCollection

Removes and releases all keys and objects within the dictionary.

free

Deallocates or releases any resources used by the OSDictionary instance.

getCapacity

Returns the number of objects the dictionary can store without reallocating.

getCapacityIncrement

Returns the storage increment of the dictionary.

getCount

Returns the current number of key/object pairs contained within the dictionary.

getObject

Returns the object stored under a given key.

getObject(const OSString *)

Returns the object stored under a given key.

getObject(const OSSymbol *)

Returns the object stored under a given key.

initWithCapacity

Initializes a new instance of OSDictionary.

initWithDictionary

Initializes a new OSDictionary with the contents of another dictionary.

initWithObjects(const OSObject *, const OSString *, unsigned int, unsigned int)

Initializes a new OSDictionary with keys and objects provided.

initWithObjects(const OSObject *, const OSSymbol *, unsigned int, unsigned int)

Initializes a new OSDictionary with keys and objects provided.

isEqualTo

Tests the equality of an OSDictionary to an arbitrary object.

isEqualTo(const OSDictionary *)

Tests the equality of two OSDictionary objects.

isEqualTo(const OSDictionary *, const OSCollection *)

Tests the equality of two OSDictionary objects over a subset of keys.

merge

Merges the contents of a dictionary into the receiver.

removeObject

Removes a key/object pair from the dictionary.

removeObject(const OSString *)

Removes a key/object pair from the dictionary.

removeObject(const OSSymbol *)

Removes a key/object pair from the dictionary.

serialize

Archives the receiver into the provided OSSerialize object.

setCapacityIncrement

Sets the storage increment of the dictionary.

setObject

Stores an object in the dictionary under a key.

setObject(const OSString *, const OSMetaClassBase *)

Stores an object in the dictionary under a key.

setObject(const OSSymbol *, const OSMetaClassBase *)

Stores an object in the dictionary under a key.

withCapacity

Creates and initializes an empty OSDictionary.

withDictionary

Creates and initializes an OSDictionary populated with the contents of another dictionary.

withObjects(const OSObject *, const OSString *, unsigned int, unsigned int)

Creates and initializes an OSDictionary populated with keys and objects provided.

withObjects(const OSObject *, const OSSymbol *, unsigned int, unsigned int)

Creates and initializes an OSDictionary populated with keys and objects provided.

### Instance Methods

- copyCollection

- ensureCapacity

Allocates capacity for members in dictionary.

- flushCollection

Removes and drops references to all members of dictionary.

- free

- getCapacity

Returns count of currently allocated capacity for members in dictionary.

- getCapacityIncrement

- getCount

Returns count of members in dictionary.

- getMetaClass

- getNextObjectForIterator

- getObject

- getObject

Returns a member of the dictionary.

- getObject

Returns a member of the dictionary.

- initIterator

- initWithCapacity

- initWithDictionary

- initWithObjects

- initWithObjects

- isEqualTo

Compares certain members of two dictionaries with isEqualTo().

- isEqualTo

Compares all members of two dictionaries with isEqualTo().

- isEqualTo

Compares the dictionary with an OSObject

- iterateObjects

- iterateObjects

- iteratorSize

- merge

Adds all members of a dictionary to this dictionary.

- removeObject

- removeObject

Remove an object by key from the dictionary.

- removeObject

Remove an object by key from the dictionary.

- serialize

- setCapacityIncrement

- setObject

- setObject

Add or replace an object in the dictionary.

- setObject

Add or replace an object in the dictionary.

- setObject

- setObject

- setObject

- setOptions

Recursively sets option bits in the dictionary and all child collections.

### Type Methods

+ withCapacity

Allocates an OSDictionary object with preallocated capacity.

+ withDictionary

Allocates an OSDictionary object with given members and preallocated capacity.

+ withObjects

+ withObjects

Allocates an OSDictionary object with given members and preallocated capacity.

## Relationships

### Inherits From

- OSCollection

## See Also

### Collections

OSArray

OSArray provides an indexed store of objects.

OSSet

OSSet provides an unordered set store of objects.

OSOrderedSet

OSOrderedSet provides an ordered set store of objects.

OSCollection

The abstract superclass for Libkern collections.

OSCollectionIterator

OSIterator

The abstract superclass for Libkern iterators.

