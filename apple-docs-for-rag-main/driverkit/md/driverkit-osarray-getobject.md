

- DriverKit
- OSArray
-  getObject 

Instance Method

# getObject

Returns a member of the array.

DriverKitiOSiPadOSmacOS

``` source
OSObject * getObject(uint32_t index) const;
```

## Parameters 

`index`  

Zero based index less than the array count to add the object.

## Return Value

Member at the given index or NULL if the index is greater or equal to the array count. The retain count of the result object is not incremented and the object should not be release by the caller.

## Discussion

If the index is less than the array count the member at that index is returned, with no additional retain count (the caller should not release). Otherwise NULL.

## See Also

### Accessing Elements

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

removeObject

Removes a current member of the array.

OSArrayAppendValue

OSArrayReplaceValue

