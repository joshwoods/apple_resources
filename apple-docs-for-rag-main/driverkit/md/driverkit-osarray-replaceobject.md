

- DriverKit
- OSArray
-  replaceObject 

Instance Method

# replaceObject

Removes a current member of the array and replaces it with another object.

DriverKitiOSiPadOSmacOS

``` source
bool replaceObject(uint32_t index, const OSMetaClassBase * anObject);
```

## Parameters 

`index`  

Zero based index less than the array count to add the object.

`anObject`  

Object to be added to the array.

## Return Value

True on success, which retains the added object and releases the current member, or false on failure which does not retain the object and leaves the current member.

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

removeObject

Removes a current member of the array.

OSArrayAppendValue

OSArrayReplaceValue

