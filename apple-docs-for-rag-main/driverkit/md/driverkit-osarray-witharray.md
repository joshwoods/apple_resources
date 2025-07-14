

- DriverKit
- OSArray
-  withArray 

Static Method

# withArray

Allocates an OSArray object with given members and preallocated capacity.

DriverKitiOSiPadOSmacOS

``` source
static OSArrayPtr withArray(const OSArray * array, uint32_t capacity);
```

## Parameters 

`array`  

Array object containing members for the new array.

`capacity`  

Count of allocated capacity for members in array.

## Return Value

NULL on failure, otherwise the allocated OSArray with reference count 1 to be released by the caller.

## See Also

### Creating an Array

withCapacity

Allocates an OSArray object with preallocated capacity.

withObjects

Allocates an OSArray object with given members and preallocated capacity.

OSArrayCreate

merge

Appends all members of an array to this array.

free

flushCollection

Removes and drops references to all members of array.

