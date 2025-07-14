

- DriverKit
- OSArray
-  getNextIndexOfObject 

Instance Method

# getNextIndexOfObject

Searches the array for an object.

DriverKitiOSiPadOSmacOS

``` source
uint32_t getNextIndexOfObject(const OSMetaClassBase * anObject, uint32_t index) const;
```

## Parameters 

`anObject`  

The object to search for.

`index`  

Zero based index less than the array count to begin the search.

## Return Value

Index at which the object was found, or -1U if the member was not found in the array after the index parameter.

## Discussion

Beginning at the passed index, iterate the array until the object instance is found or there are no more members. The search is done by pointer equality.

## See Also

### Accessing Elements

getObject

Returns a member of the array.

getLastObject

Returns the last member of the array.

setObject

Appends an object as the last member of the array.

setObject

Sets an object as the member of the array at a given index.

iterateObjects

Iterates the array calling a callback block for each member.

replaceObject

Removes a current member of the array and replaces it with another object.

removeObject

Removes a current member of the array.

OSArrayAppendValue

OSArrayReplaceValue

