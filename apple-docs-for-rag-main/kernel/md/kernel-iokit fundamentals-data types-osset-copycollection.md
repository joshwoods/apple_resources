

- Kernel
- IOKit Fundamentals
- Data Types
- OSSet
-  copyCollection 

# copyCollection

Creates a deep copy of this set and its child collections.

``` source
OSCollection *copyCollection(
 OSDictionary *cycleDict = 0); 
```

## Parameters 

`cycleDict`  

A dictionary of all of the collections that have been copied so far, which is used to track circular references. To start the copy at the top level, pass `NULL`.

## Return Value

The newly copied set, with a retain count of 1, or `NULL` if there is insufficient memory to do the copy.

## Overview

The receiving set, and any collections it contains, recursively, are copied. Objects that are not derived from OSCollection are retained rather than copied.

## See Also

### Miscellaneous

containsObject

Checks the set for the presence of an object.

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

