

- Kernel
- IOKit Fundamentals
- Data Types
- OSSet
-  withArray 

# withArray

Creates and initializes an OSSet populated with the contents of an OSArray.

``` source
static OSSet * withArray( 
 const OSArray *array, 
 unsigned int capacity = 0); 
```

## Parameters 

`array`  

An array whose objects will be stored in the new OSSet.

`capacity`  

The initial storage capacity of the new set object. If 0, the capacity is set to the number of objects in `array`; otherwise `capacity` must be greater than or equal to the number of objects in `array`.

## Return Value

An instance of OSSet containing the objects of `array`, with a retain count of 1; `NULL` on failure.

## Overview

Each distinct object in `array` is added to the new set.

`array` must be non-`NULL`. If `capacity` is nonzero, it must be greater than or equal to `count`. The new OSSet will grow as needed to accommodate more key-object pairs (*unlike*`CFMutableSet`, for which the initial capacity is a hard limit).

The objects in `array` are retained for storage in the new set, not copied.

## See Also

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

withCapacity

Creates and initializes an empty OSSet.

withObjects

Creates and initializes an OSSet populated with objects provided.

withSet

Creates and initializes an OSSet populated with the contents of another OSSet.

