

- Kernel
- IOKit Fundamentals
- Data Types
-  OSArray 

Class

# OSArray

OSArray provides an indexed store of objects.

macOS 10.0+

``` source
class OSArray : OSCollection
```

## Overview

OSArray is a container for Libkern C++ objects (those derived from OSMetaClassBase, in particular OSObject). Storage and access are by array index.

You must generally cast retrieved objects from OSObject to the desired class using OSDynamicCast. This macro returns the object cast to the desired class, or `NULL` if the object isn't derived from that class.

As with all Libkern collection classes, OSArray retains objects added to it, and releases objects removed from it (or replaced). An OSArray also grows as necessary to accommodate new objects, *unlike* Core Foundation collections (it does not, however, shrink).

**Use Restrictions**

With very few exceptions in the I/O Kit, all Libkern-based C++ classes, functions, and macros are **unsafe** to use in a primary interrupt context. Consult the I/O Kit documentation related to primary interrupts for more information.

OSArray provides no concurrency protection; it's up to the usage context to provide any protection necessary. Some portions of the I/O Kit, such as IORegistryEntry, handle synchronization via defined member functions for setting properties.

## Topics

### Miscellaneous

copyCollection

Creates a deep copy of an array and its child collections.

ensureCapacity

Ensures the array has enough space to store the requested number of objects.

flushCollection

Removes and releases all objects within the array.

free

Deallocates or releases any resources used by the OSArray instance.

getCapacity

Returns the number of objects the array can store without reallocating.

getCapacityIncrement

Returns the storage increment of the array.

getCount

Returns the current number of objects within the array.

getLastObject

Returns the last object in the array.

getNextIndexOfObject

Scans the array for the next instance of a specific object at or beyond a given index.

getObject

Return the object stored at a given index.

initWithArray

Initializes a new OSArray populated with the contents of another array.

initWithCapacity

Initializes a new instance of OSArray.

initWithObjects

Initializes a new OSArray populated with objects provided.

isEqualTo(const OSArray *)

Tests the equality of two OSArray objects.

isEqualTo(const OSMetaClassBase *)

Tests the equality of an OSArray to an arbitrary object.

merge

Appends the contents of an array onto the receiving array.

removeObject

Removes an object from the array.

replaceObject

Replaces an object in an array at a given index.

serialize

Archives the receiver into the provided OSSerialize object.

setCapacityIncrement

Sets the storage increment of the array.

setObject(const OSMetaClassBase *)

Appends an object onto the end of the array, increasing storage if necessary.

setObject(unsigned int, const OSMetaClassBase *)

Inserts or appends an object into the array at a particular index.

withArray

Creates and initializes an OSArray populated with the contents of another array.

withCapacity

Creates and initializes an empty OSArray.

withObjects

Creates and initializes an OSArray populated with objects provided.

### Instance Methods

- copyCollection

- ensureCapacity

Allocates capacity for members in array.

- flushCollection

Removes and drops references to all members of array.

- free

- getCapacity

Returns count of currently allocated capacity for members in array.

- getCapacityIncrement

- getCount

Returns count of members in array.

- getLastObject

Returns the last member of the array.

- getMetaClass

- getNextIndexOfObject

Searches the array for an object.

- getNextObjectForIterator

- getObject

Returns a member of the array.

- initIterator

- initWithArray

- initWithCapacity

- initWithObjects

- isEqualTo

Compares all members of two arrays with isEqualTo().

- isEqualTo

Compares the array with an OSObject

- iteratorSize

- merge

Appends all members of an array to this array.

- removeObject

Removes a current member of the array.

- replaceObject

Removes a current member of the array and replaces it with another object.

- replaceObject

- serialize

- setCapacityIncrement

- setObject

Appends an object as the last member of the array.

- setObject

Sets an object as the member of the array at a given index.

- setObject

- setObject

- setOptions

Recursively sets option bits in an array and all child collections.

### Type Methods

+ withArray

Allocates an OSArray object with given members and preallocated capacity.

+ withCapacity

Allocates an OSArray object with preallocated capacity.

+ withObjects

Allocates an OSArray object with given members and preallocated capacity.

## Relationships

### Inherits From

- OSCollection

## See Also

### Collections

OSDictionary

OSDictionary provides an associative store using strings for keys.

OSSet

OSSet provides an unordered set store of objects.

OSOrderedSet

OSOrderedSet provides an ordered set store of objects.

OSCollection

The abstract superclass for Libkern collections.

OSCollectionIterator

OSIterator

The abstract superclass for Libkern iterators.

