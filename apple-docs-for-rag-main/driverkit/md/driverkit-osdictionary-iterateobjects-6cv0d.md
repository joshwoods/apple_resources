

- DriverKit
- OSDictionary
-  iterateObjects 

Instance Method

# iterateObjects

Iterates the dictionary calling a callback block for each member.

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

Calls the block with each member of the dictionary. The block must not dictionary the array during iteration. If the block returns true the iteration continues for all members, returning false halts the iteration early. OSDictionary also has a dictionary specific iterateObjects() which supplies the key and value to the callback.

## See Also

### Accessing Keys and Values

getObject

Returns a member of the dictionary.

getObject

Returns a member of the dictionary.

setObject

Add or replace an object in the dictionary.

setObject

Add or replace an object in the dictionary.

removeObject

Remove an object by key from the dictionary.

removeObject

Remove an object by key from the dictionary.

iterateObjects

Iterates the dictionary calling a callback block for each member.

OSDictionaryIterateObjectsBlock

OSDictionaryIterateObjectsCallback

