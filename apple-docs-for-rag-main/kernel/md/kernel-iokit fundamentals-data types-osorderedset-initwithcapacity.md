

- Kernel
- IOKit Fundamentals
- Data Types
- OSOrderedSet
-  initWithCapacity 

# initWithCapacity

Initializes a new instance of OSOrderedSet.

``` source
virtual bool initWithCapacity( 
 unsigned int capacity, 
 OSOrderFunction orderFunc = 0, 
 void *orderingContext = 0); 
```

## Parameters 

`capacity`  

The initial storage capacity of the new ordered set object.

`orderFunc`  

A C function that implements the sorting algorithm for the set.

`orderingContext`  

An ordering context, which is passed to `orderFunc`.

## Return Value

`true` on success, `false` on failure.

## Overview

Not for general use. Use the static instance creation method withCapacity instead.

`capacity` must be nonzero. The new set will grow as needed to accommodate more key/object pairs (*unlike* Core Foundation collections, for which the initial capacity is a hard limit).

If `orderFunc` is provided, it is used by setObject(const OSMetaClassBase \*) to determine where to insert a new object. Other object-setting functions ignore ordering.

`orderingContext` is not retained or otherwise memory-managed by the ordered set. If it needs to be deallocated, you must track references to it and the ordered set in order to deallocate it appropriately. See getOrderingRef.

## See Also

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

