

- DriverKit
- OSDictionary
-  getObject 

Instance Method

# getObject

Returns a member of the dictionary.

DriverKitiOSiPadOSmacOS

``` source
OSObject * getObject(const char * aKey) const;
```

## Parameters 

`aKey`  

A c-string key. An OSString is created from aKey and used as the key for the dictionary.

## Return Value

Member at the given index or NULL if the index is greater or equal to the array count. The retain count of the result object is not incremented and the object should not be release by the caller.

## Discussion

Looks up an existing object in the dictionary with the given key and returns it.

## See Also

### Accessing Keys and Values

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

iterateObjects

Iterates the dictionary calling a callback block for each member.

OSDictionaryIterateObjectsBlock

OSDictionaryIterateObjectsCallback

