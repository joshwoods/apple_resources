

- DriverKit
- OSArray
-  iterateObjects 

Instance Method

# iterateObjects

Iterates the array calling a callback block for each member.

DriverKitiOSiPadOSmacOS

``` source
bool iterateObjects(OSCollectionIterateObjectsBlockblock) const;
```

## Parameters 

`block`  

The block to invoke.

## Return Value

False if the callback block returned false, otherwise true (including if the array is empty).

## Discussion

Calls the block with each member of the array, starting at index zero. The block must not modify the array during iteration. If the block returns true the iteration continues for all members, returning false halts the iteration early.

## See Also

### Accessing Elements

getObject

Returns a member of the array.

getLastObject

Returns the last member of the array.

getNextIndexOfObject

Searches the array for an object.

setObject

Appends an object as the last member of the array.

setObject

Sets an object as the member of the array at a given index.

replaceObject

Removes a current member of the array and replaces it with another object.

removeObject

Removes a current member of the array.

OSArrayAppendValue

OSArrayReplaceValue

