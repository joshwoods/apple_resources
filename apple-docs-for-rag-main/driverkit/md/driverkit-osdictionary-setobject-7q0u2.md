

- DriverKit
- OSDictionary
-  setObject 

Instance Method

# setObject

Add or replace an object in the dictionary.

DriverKitiOSiPadOSmacOS

``` source
bool setObject(const char * aKey, const OSMetaClassBase * anObject);
```

## Parameters 

`aKey`  

A c-string key. An OSString is created from aKey and used as the key for the dictionary.

`anObject`  

Object to be added to the dictionary.

## Return Value

True on success, which retains the object, or false on failure which does not retain the object.

## Discussion

The object is added to the dictionary with the key object. If an object with the given key existed prior to the call it is replaced and released. The dictionary capacity will be grown if necessary.

## See Also

### Accessing Keys and Values

getObject

Returns a member of the dictionary.

getObject

Returns a member of the dictionary.

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

