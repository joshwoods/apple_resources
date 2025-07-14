

- Kernel
- IOKit Fundamentals
- Data Types
- OSDictionary
-  isEqualTo(const OSDictionary \*, const OSCollection \*) 

# isEqualTo(const OSDictionary \*, const OSCollection \*)

Tests the equality of two OSDictionary objects over a subset of keys.

``` source
virtual bool isEqualTo( 
 const OSDictionary *aDictionary, 
 const OSCollection *keys) const; 
```

## Parameters 

`aDictionary`  

The dictionary to be compared against the receiver.

`keys`  

An OSArray or OSDictionary containing the keys (as `OSString` or OSSymbol) describing the intersection for the comparison.

## Return Value

`true` if the intersections of the two dictionaries are equal.

## Overview

Two OSDictionary objects are considered equal by this function if both have objects stored for all keys provided, and if the objects stored in each under a given key compare as equal using isEqualTo.

## See Also

### Miscellaneous

copyCollection

Creates a deep copy of the dictionary and its child collections.

ensureCapacity

Ensures the dictionary has enough space to store the requested number of key/object pairs.

flushCollection

Removes and releases all keys and objects within the dictionary.

free

Deallocates or releases any resources used by the OSDictionary instance.

getCapacity

Returns the number of objects the dictionary can store without reallocating.

getCapacityIncrement

Returns the storage increment of the dictionary.

getCount

Returns the current number of key/object pairs contained within the dictionary.

getObject

Returns the object stored under a given key.

getObject(const OSString *)

Returns the object stored under a given key.

getObject(const OSSymbol *)

Returns the object stored under a given key.

initWithCapacity

Initializes a new instance of OSDictionary.

initWithDictionary

Initializes a new OSDictionary with the contents of another dictionary.

initWithObjects(const OSObject *, const OSString *, unsigned int, unsigned int)

Initializes a new OSDictionary with keys and objects provided.

initWithObjects(const OSObject *, const OSSymbol *, unsigned int, unsigned int)

Initializes a new OSDictionary with keys and objects provided.

isEqualTo

Tests the equality of an OSDictionary to an arbitrary object.

isEqualTo(const OSDictionary *)

Tests the equality of two OSDictionary objects.

merge

Merges the contents of a dictionary into the receiver.

removeObject

Removes a key/object pair from the dictionary.

removeObject(const OSString *)

Removes a key/object pair from the dictionary.

removeObject(const OSSymbol *)

Removes a key/object pair from the dictionary.

serialize

Archives the receiver into the provided OSSerialize object.

setCapacityIncrement

Sets the storage increment of the dictionary.

setObject

Stores an object in the dictionary under a key.

setObject(const OSString *, const OSMetaClassBase *)

Stores an object in the dictionary under a key.

setObject(const OSSymbol *, const OSMetaClassBase *)

Stores an object in the dictionary under a key.

withCapacity

Creates and initializes an empty OSDictionary.

withDictionary

Creates and initializes an OSDictionary populated with the contents of another dictionary.

withObjects(const OSObject *, const OSString *, unsigned int, unsigned int)

Creates and initializes an OSDictionary populated with keys and objects provided.

withObjects(const OSObject *, const OSSymbol *, unsigned int, unsigned int)

Creates and initializes an OSDictionary populated with keys and objects provided.

