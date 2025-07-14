

- Kernel
- IOKit Fundamentals
- Data Types
-  OSSet 

Class

# OSSet

OSSet provides an unordered set store of objects.

DriverKitKernelDriverKit 21.0+macOS 10.0+

**DriverKit**

``` source
class OSSet : OSArray
```

**macOS**

``` source
class OSSet : OSCollection
```

## Overview

OSSet is a container for Libkern C++ objects (those derived from OSMetaClassBase, in particular OSObject). Storage and access follow basic set logic: you can add or remove an object, and test whether the set contains a particular object. A given object is only stored in the set once, and there is no ordering of objects in the set. A subclass OSOrderedSet, provides for ordered set logic.

As with all Libkern collection classes, OSSet retains objects added to it, and releases objects removed from it. An OSSet also grows as necessary to accommodate new objects, *unlike* Core Foundation collections (it does not, however, shrink).

**Use Restrictions**

With very few exceptions in the I/O Kit, all Libkern-based C++ classes, functions, and macros are **unsafe** to use in a primary interrupt context. Consult the I/O Kit documentation related to primary interrupts for more information.

OSSet provides no concurrency protection; it's up to the usage context to provide any protection necessary. Some portions of the I/O Kit, such as IORegistryEntry, handle synchronization via defined member functions for setting properties.

## Topics

### Miscellaneous

containsObject

Checks the set for the presence of an object.

copyCollection

Creates a deep copy of this set and its child collections.

ensureCapacity

Ensures the set has enough space to store the requested number of distinct objects.

flushCollection

Removes and releases all objects within the set.

free

Deallocates or releases any resources used by the OSSet instance.

getAnyObject

Returns an arbitrary (not random) object from the set.

getCapacity

Returns the number of objects the set can store without reallocating.

getCapacityIncrement

Returns the storage increment of the set.

getCount

Returns the current number of objects within the set.

initWithArray

Initializes a new OSSet populated with the contents of an OSArray.

initWithCapacity

Initializes a new instance of OSSet.

initWithObjects

Initializes a new OSSet populated with objects provided.

initWithSet

Initializes a new OSSet populated with the contents of another OSSet.

isEqualTo(const OSMetaClassBase *)

Tests the equality of an OSSet against an arbitrary object.

isEqualTo(const OSSet *)

Tests the equality of two OSSet objects.

member

Checks the set for the presence of an object.

merge(const OSArray *)

Adds the contents of an OSArray to the set.

merge(const OSSet *)

Adds the contents of an OSet to the set.

removeObject

Removes an object from the set.

serialize

Archives the receiver into the provided OSSerialize object.

setCapacityIncrement

Sets the storage increment of the set.

setObject

Adds an object to the OSSet if it is not already present.

withArray

Creates and initializes an OSSet populated with the contents of an OSArray.

withCapacity

Creates and initializes an empty OSSet.

withObjects

Creates and initializes an OSSet populated with objects provided.

withSet

Creates and initializes an OSSet populated with the contents of another OSSet.

### Instance Methods

- containsObject

- copyCollection

- ensureCapacity

- flushCollection

- free

- getAnyObject

- getCapacity

- getCapacityIncrement

- getCount

- getMetaClass

- getNextObjectForIterator

- init

- initIterator

- initWithArray

- initWithCapacity

- initWithObjects

- initWithSet

- isEqualTo

- isEqualTo

- iteratorSize

- member

- merge

- merge

- removeObject

- removeObject

- serialize

- setCapacityIncrement

- setObject

- setObject

- setOptions

Recursively sets option bits in the set and all child collections.

### Type Methods

+ withArray

+ withCapacity

+ withObjects

+ withSet

## Relationships

### Inherits From

- OSArray
- OSCollection

## See Also

### Collections

OSArray

OSArray provides an indexed store of objects.

OSDictionary

OSDictionary provides an associative store using strings for keys.

OSOrderedSet

OSOrderedSet provides an ordered set store of objects.

OSCollection

The abstract superclass for Libkern collections.

OSCollectionIterator

OSIterator

The abstract superclass for Libkern iterators.

