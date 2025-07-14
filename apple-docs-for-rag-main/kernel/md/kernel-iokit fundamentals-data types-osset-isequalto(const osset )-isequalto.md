

- Kernel
- IOKit Fundamentals
- Data Types
- OSSet
-  isEqualTo(const OSSet \*) 

# isEqualTo(const OSSet \*)

Tests the equality of two OSSet objects.

``` source
virtual bool isEqualTo(
 const OSSet *aSet) const; 
```

## Parameters 

`aSet`  

The set object being compared against the receiver.

## Return Value

`true` if the two sets are equivalent, `false` otherwise.

## Overview

Two OSSet objects are considered equal if they have same count and the same object pointer values.

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

