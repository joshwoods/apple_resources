

- DriverKit
- OSDictionary
-  iterateObjects 

Instance Method

# iterateObjects

Iterates the dictionary calling a callback block for each member.

DriverKitiOSiPadOSmacOS

``` source
bool iterateObjects(OSDictionaryIterateObjectsBlockblock) const;
```

## Parameters 

`block`  

The block to invoke.

## Return Value

False if the callback block returned false, otherwise true (including if the dictionary is empty).

## Discussion

Calls the block with each value in the dictionary. The block must not modify the dictionary during iteration. If the block returns true the iteration continues for all members, returning false halts the iteration early.

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

