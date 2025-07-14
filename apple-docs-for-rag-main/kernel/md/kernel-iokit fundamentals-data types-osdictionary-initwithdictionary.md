

- Kernel
- IOKit Fundamentals
- Data Types
- OSDictionary
-  initWithDictionary 

# initWithDictionary

Initializes a new OSDictionary with the contents of another dictionary.

``` source
virtual bool initWithDictionary( 
 const OSDictionary *dict, 
 unsigned int capacity = 0); 
```

## Parameters 

`dict`  

A dictionary whose contents will be placed in the new instance.

`capacity`  

The initial storage capacity of the new dictionary object. If 0, the capacity is set to the number of key/value pairs in `dict`; otherwise `capacity` must be greater than or equal to the number of key/value pairs in `dict`.

## Return Value

`true` on success, `false` on failure.

## Overview

Not for general use. Use the static instance creation method withDictionary instead.

`dict` must be non-`NULL`. If `capacity` is nonzero, it must be greater than or equal to `count`. The new dictionary will grow as needed to accommodate more key/object pairs (*unlike*`CFMutableDictionary`, for which the initial capacity is a hard limit).

The keys and objects in `dict` are retained for storage in the new OSDictionary, not copied.

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

withObjects(const OSObject *, const OSString *, unsigned int, unsigned int)

Creates and initializes an OSDictionary populated with keys and objects provided.

withObjects(const OSObject *, const OSSymbol *, unsigned int, unsigned int)

Creates and initializes an OSDictionary populated with keys and objects provided.

