

- DriverKit
- OSArray
-  getLastObject 

Instance Method

# getLastObject

Returns the last member of the array.

DriverKitiOSiPadOSmacOS

``` source
OSObject * getLastObject() const;
```

## Return Value

Member at the last index or NULL if array has no members.

## Discussion

If the array has non-zero count the member at the last index is returned, with no additional retain count (the caller should not release). Otherwise NULL.

## See Also

### Accessing Elements

getObject

Returns a member of the array.

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

