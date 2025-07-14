

- DriverKit
- OSArray
-  merge 

Instance Method

# merge

Appends all members of an array to this array.

DriverKitiOSiPadOSmacOS

``` source
bool merge(const OSArray * otherArray);
```

## Parameters 

`otherArray`  

All members of thie array will be appended to the array.

## Return Value

True on success, which retains all the added objects, or false on failure which does not retain the objects.

## Discussion

Appends all members of an array to this array. The array capacity will be grown if necessary.

## See Also

### Creating an Array

withArray

Allocates an OSArray object with given members and preallocated capacity.

withCapacity

Allocates an OSArray object with preallocated capacity.

withObjects

Allocates an OSArray object with given members and preallocated capacity.

OSArrayCreate

free

flushCollection

Removes and drops references to all members of array.

