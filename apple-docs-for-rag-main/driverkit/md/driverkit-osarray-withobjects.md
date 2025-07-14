

- DriverKit
- OSArray
-  withObjects 

Static Method

# withObjects

Allocates an OSArray object with given members and preallocated capacity.

DriverKitiOSiPadOSmacOS

``` source
static OSArrayPtr withObjects(const OSObject * * values, uint32_t count, uint32_t capacity);
```

## Parameters 

`values`  

C-array pointer to members for the array.

`count`  

Count of members being added to the array.

`capacity`  

Count of allocated capacity for members in array.

## Return Value

NULL on failure, otherwise the allocated OSArray with reference count 1 to be released by the caller.

## See Also

### Creating an Array

withArray

Allocates an OSArray object with given members and preallocated capacity.

withCapacity

Allocates an OSArray object with preallocated capacity.

OSArrayCreate

merge

Appends all members of an array to this array.

free

flushCollection

Removes and drops references to all members of array.

