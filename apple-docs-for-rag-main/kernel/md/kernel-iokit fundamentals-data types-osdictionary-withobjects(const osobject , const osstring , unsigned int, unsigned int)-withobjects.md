

- Kernel
- IOKit Fundamentals
- Data Types
- OSDictionary
-  withObjects(const OSObject \*, const OSString \*, unsigned int, unsigned int) 

# withObjects(const OSObject \*, const OSString \*, unsigned int, unsigned int)

Creates and initializes an OSDictionary populated with keys and objects provided.

``` source
static OSDictionary * withObjects( 
 const OSObject *objects[], 
 const OSString *keys[], 
 unsigned int count, 
 unsigned int capacity = 0); 
```

## Parameters 

`objects`  

A C array of OSMetaClassBase-derived objects.

`keys`  

A C array of OSString keys for the corresponding objects in `objects`.

`count`  

The number of keys and objects to be placed into the dictionary.

`capacity`  

The initial storage capacity of the new dictionary object. If 0, `count` is used; otherwise this value must be greater than or equal to `count`.

## Return Value

An instance of OSDictionary containing the key/object pairs provided, with a retain count of 1; `NULL` on failure.

## Overview

`objects` and `keys` must be non-`NULL`, and `count` must be nonzero. If `capacity` is nonzero, it must be greater than or equal to `count`. The new dictionary will grow as needed to accommodate more key/object pairs (*unlike*`CFMutableDictionary`, for which the initial capacity is a hard limit).

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

isEqualTo(const OSDictionary *, const OSCollection *)

Tests the equality of two OSDictionary objects over a subset of keys.

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

withObjects(const OSObject *, const OSSymbol *, unsigned int, unsigned int)

Creates and initializes an OSDictionary populated with keys and objects provided.

