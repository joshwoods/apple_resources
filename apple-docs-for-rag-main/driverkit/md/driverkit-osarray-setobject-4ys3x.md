

- DriverKit
- OSArray
-  setObject 

Instance Method

# setObject

Sets an object as the member of the array at a given index.

DriverKitiOSiPadOSmacOS

``` source
bool setObject(uint32_t index, const OSMetaClassBase * anObject);
```

## Parameters 

`index`  

Zero based index less than or equal to the array count to add the object.

`anObject`  

Object to be added to the array.

## Return Value

True on success, which retains the object, or false on failure which does not retain the object.

## Discussion

Sets an object as the member of the array at a given index. The array capacity will be grown if necessary.

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

iterateObjects

Iterates the array calling a callback block for each member.

replaceObject

Removes a current member of the array and replaces it with another object.

removeObject

Removes a current member of the array.

OSArrayAppendValue

OSArrayReplaceValue

