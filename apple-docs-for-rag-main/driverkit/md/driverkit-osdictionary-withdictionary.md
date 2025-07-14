

- DriverKit
- OSDictionary
-  withDictionary 

Static Method

# withDictionary

Allocates an OSDictionary object with given members and preallocated capacity.

DriverKitiOSiPadOSmacOS

``` source
static OSDictionaryPtr withDictionary(const OSDictionary * dictionary, uint32_t capacity);
```

## Parameters 

`dictionary`  

Dictionary object containing members for the new dictionary.

`capacity`  

Count of allocated capacity for members in array.

## Return Value

NULL on failure, otherwise the allocated OSDictionary with reference count 1 to be released by the caller.

## See Also

### Creating a Dictionary

withCapacity

Allocates an OSDictionary object with preallocated capacity.

withObjects

Allocates an OSDictionary object with given members and preallocated capacity.

OSDictionaryCreate

merge

Adds all members of a dictionary to this dictionary.

free

flushCollection

Removes and drops references to all members of dictionary.

