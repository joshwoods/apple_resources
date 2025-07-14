

- Kernel
- IOKit Fundamentals
- Data Types
-  OSOrderedSet 

Class

# OSOrderedSet

OSOrderedSet provides an ordered set store of objects.

DriverKitKernelDriverKit 21.0+macOS 10.0+

**DriverKit**

``` source
class OSOrderedSet : OSSet
```

**macOS**

``` source
class OSOrderedSet : OSCollection
```

## Overview

OSOrderedSet is a container for Libkern C++ objects (those derived from OSMetaClassBase, in particular OSObject). Storage and access follow ordered set logic. A given object is stored in the set only once, but you can:

- Define a sorting function for automated ordering (upon addition only)

- Manually insert new objects in the set (overriding sorting)

- Add and remove objects in the set

- Test whether the set contains a particular object

- Get the object stored at a particular index.

Note that automated ordering is performed only upon addition of objects and depends on the existing objects being properly sorted. There is no function to re-sort the contents of an OSOrderedSet or to change the ordering function. In general, you should either use the one ordered-insertion function, or the indexed-insertion functions, and not mix the two.

As with all Libkern collection classes, OSOrderedSet retains objects added to it, and releases objects removed from it. An OSOrderedSet also grows as necessary to accommodate new objects, *unlike* Core Foundation collections (it does not, however, shrink).

### Use Restrictions

With very few exceptions in the I/O Kit, all Libkern-based C++ classes, functions, and macros are **unsafe** to use in a primary interrupt context. Consult the I/O Kit documentation related to primary interrupts for more information.

OSOrderedSet provides no concurrency protection; it's up to the usage context to provide any protection necessary. Some portions of the I/O Kit, such as IORegistryEntry, handle synchronization via defined member functions for setting properties.

## Topics

### Miscellaneous

containsObject

Checks the ordered set for the presence of an object.

copyCollection

Creates a deep copy of this ordered set and its child collections.

ensureCapacity

Ensures the set has enough space to store the requested number of distinct objects.

flushCollection

Removes and releases all objects within the ordered set.

free

Deallocatesand releases any resources used by the OSOrderedSet instance.

getCapacity

Returns the number of objects the ordered set can store without reallocating.

getCapacityIncrement

Returns the storage increment of the ordered set.

getCount

Returns the current number of objects within the ordered set.

getFirstObject

The object at index 0 in the ordered set if there is one, otherwise `NULL`.

getLastObject

The last object in the ordered set if there is one, otherwise `NULL`.

getObject

Gets the object at a particular index.

getOrderingRef

Returns the ordering context the ordered set was created with.

initWithCapacity

Initializes a new instance of OSOrderedSet.

isEqualTo(const OSMetaClassBase *)

Tests the equality of an OSOrderedSet against an arbitrary object.

isEqualTo(const OSOrderedSet *)

Tests the equality of two OSOrderedSet objects.

member

Checks the ordered set for the presence of an object.

orderObject

Calls the ordered set's order function against a `NULL` object.

removeObject

Removes an object from the ordered set.

setCapacityIncrement

Sets the storage increment of the ordered set.

setFirstObject

Adds an object to the OSOrderedSet at index 0 if it is not already present.

setLastObject

Adds an object at the end of the OSOrderedSet if it is not already present.

setObject(const OSMetaClassBase *)

Adds an object to the OSOrderedSet if it is not already present, storing it in sorted order if there is an order function.

setObject(unsigned int, const OSMetaClassBase *)

Adds an object to an OSOrderedSet at a specified index if it is not already present.

withCapacity

Creates and initializes an empty OSOrderedSet.

### Callbacks

OSOrderFunction

The sorting function used by an OSOrderedSet to order objects.

### Instance Methods

- containsObject

- copyCollection

- ensureCapacity

- flushCollection

- free

- getCapacity

- getCapacityIncrement

- getCount

- getFirstObject

- getLastObject

- getMetaClass

- getNextObjectForIterator

- getObject

- getOrderingRef

- init

- initIterator

- initWithCapacity

- isEqualTo

- isEqualTo

- iteratorSize

- member

- orderObject

- removeObject

- removeObject

- setCapacityIncrement

- setFirstObject

- setFirstObject

- setLastObject

- setLastObject

- setObject

- setObject

- setObject

- setObject

- setOptions

### Type Methods

+ withCapacity

+ withCapacity

## Relationships

### Inherits From

- OSCollection
- OSSet

## See Also

### Collections

OSArray

OSArray provides an indexed store of objects.

OSDictionary

OSDictionary provides an associative store using strings for keys.

OSSet

OSSet provides an unordered set store of objects.

OSCollection

The abstract superclass for Libkern collections.

OSCollectionIterator

OSIterator

The abstract superclass for Libkern iterators.

