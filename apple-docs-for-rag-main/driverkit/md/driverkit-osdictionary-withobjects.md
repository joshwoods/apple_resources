

- DriverKit
- OSDictionary
-  withObjects 

Static Method

# withObjects

Allocates an OSDictionary object with given members and preallocated capacity.

DriverKitiOSiPadOSmacOS

``` source
static OSDictionaryPtr withObjects(const OSObject * * values, const OSObject * * keys, uint32_t count, uint32_t capacity);
```

## Parameters 

`values`  

C-array pointer to values for the dictionary.

`keys`  

C-array pointer to keys for the dictionary.

`count`  

Count of members being added to the dictionary.

`capacity`  

Count of allocated capacity for members in dictionary.

## Return Value

NULL on failure, otherwise the allocated OSDictionary with reference count 1 to be released by the caller.

## See Also

### Creating a Dictionary

withCapacity

Allocates an OSDictionary object with preallocated capacity.

withDictionary

Allocates an OSDictionary object with given members and preallocated capacity.

OSDictionaryCreate

merge

Adds all members of a dictionary to this dictionary.

free

flushCollection

Removes and drops references to all members of dictionary.

