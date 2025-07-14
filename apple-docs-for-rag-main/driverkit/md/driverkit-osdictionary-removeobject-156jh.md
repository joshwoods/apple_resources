

- DriverKit
- OSDictionary
-  removeObject 

Instance Method

# removeObject

Remove an object by key from the dictionary.

DriverKitiOSiPadOSmacOS

``` source
void removeObject(const char * aKey);
```

## Parameters 

`aKey`  

A c-string key. An OSString is created from aKey and used as the key for the dictionary.

## Discussion

An object in the dictionary with the given key object is removed and released.

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

iterateObjects

Iterates the dictionary calling a callback block for each member.

iterateObjects

Iterates the dictionary calling a callback block for each member.

OSDictionaryIterateObjectsBlock

OSDictionaryIterateObjectsCallback

