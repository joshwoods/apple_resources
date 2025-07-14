

- Kernel
- IOKit Fundamentals
- Data Types
- OSOrderedSet
-  setObject(const OSMetaClassBase \*) 

# setObject(const OSMetaClassBase \*)

Adds an object to the OSOrderedSet if it is not already present, storing it in sorted order if there is an order function.

``` source
virtual bool setObject(
 const OSMetaClassBase *anObject); 
```

## Parameters 

`anObject`  

The OSMetaClassBase-derived object to be added to the ordered set.

## Return Value

`true` if `anObject` was successfully added to the ordered set, `false` otherwise (including if it was already in the ordered set).

## Overview

The set adds storage to accomodate the new object, if necessary. If successfully added, the object is retained.

If `anObject` is not already in the ordered set and there is an order function, this function loops through the existing objects, calling the order function with arguments each existingObject, `anObject`, and the ordering context (or `NULL` if none was set), until the order function returns a value *greater than* or equal to 0. It then inserts `anObject` at the index of the existing object.

If there is no order function, the object is inserted at index 0.

A `false` return value can mean either that `anObject` is already present in the set, or that a memory allocation failure occurred. If you need to know whether the object is already present, use containsObject(const OSMetaClassBase \*).

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

setObject(unsigned int, const OSMetaClassBase *)

Adds an object to an OSOrderedSet at a specified index if it is not already present.

withCapacity

Creates and initializes an empty OSOrderedSet.

