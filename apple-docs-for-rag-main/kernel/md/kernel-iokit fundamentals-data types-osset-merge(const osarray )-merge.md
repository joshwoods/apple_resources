

- Kernel
- IOKit Fundamentals
- Data Types
- OSSet
-  merge(const OSArray \*) 

# merge(const OSArray \*)

Adds the contents of an OSArray to the set.

``` source
virtual bool merge(
 const OSArray *array); 
```

## Parameters 

`array`  

The OSArray object containing the objects to be added.

## Return Value

`true` if all objects from `array` are successfully added the receiver (or were already present), `false` otherwise.

## Overview

This functions adds to the receiving set all objects from `array` that are not already in the receiving set. Objects added to the receiver are retained.

In releases prior to 10.7, this function would return `false` if an object from `array` was already present in the set, or if `array` was empty. This is no longer the case, so this function correctly returns `true` when the semantic of merging is met.

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

