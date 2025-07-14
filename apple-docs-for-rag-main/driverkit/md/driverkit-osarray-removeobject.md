

- DriverKit
- OSArray
-  removeObject 

Instance Method

# removeObject

Removes a current member of the array.

DriverKitiOSiPadOSmacOS

``` source
void removeObject(uint32_t index);
```

## Parameters 

`index`  

Zero based index less than the array count of the object to remove.

## Discussion

Removes a current member of the array, shifting down all following members. The removed object is released.

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

iterateObjects

Iterates the array calling a callback block for each member.

replaceObject

Removes a current member of the array and replaces it with another object.

OSArrayAppendValue

OSArrayReplaceValue

