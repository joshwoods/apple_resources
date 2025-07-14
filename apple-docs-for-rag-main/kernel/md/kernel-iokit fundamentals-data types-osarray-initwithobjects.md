

- Kernel
- IOKit Fundamentals
- Data Types
- OSArray
-  initWithObjects 

# initWithObjects

Initializes a new OSArray populated with objects provided.

``` source
virtual bool initWithObjects( 
 const OSObject *objects[], 
 unsigned int count, 
 unsigned int capacity = 0); 
```

## Parameters 

`objects`  

A C array of OSObject-derived objects.

`count`  

The number of objects to be placed into the array.

`capacity`  

The initial storage capacity of the array object. If 0, `count` is used; otherwise this value must be greater than or equal to `count`.

## Return Value

`true` on success, `false` on failure.

## Overview

Not for general use. Use the static instance creation method withObjects instead.

`objects` must be non-`NULL`, and `count` must be nonzero. If `capacity` is nonzero, it must be greater than or equal to `count`. The new array will grow as needed to accommodate more objects (*unlike*`CFMutableArray`, for which the initial capacity is a hard limit).

## See Also

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

