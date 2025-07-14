

- DriverKit
- OSArray
-  withCapacity 

Static Method

# withCapacity

Allocates an OSArray object with preallocated capacity.

DriverKitiOSiPadOSmacOS

``` source
static OSArrayPtr withCapacity(uint32_t capacity);
```

## Parameters 

`capacity`  

Count of allocated capacity for members in array.

## Return Value

NULL on failure, otherwise the allocated OSArray with reference count 1 to be released by the caller.

## See Also

### Creating an Array

withArray

Allocates an OSArray object with given members and preallocated capacity.

withObjects

Allocates an OSArray object with given members and preallocated capacity.

OSArrayCreate

merge

Appends all members of an array to this array.

free

flushCollection

Removes and drops references to all members of array.

