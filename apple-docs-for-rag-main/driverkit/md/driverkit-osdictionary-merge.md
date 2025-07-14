

- DriverKit
- OSDictionary
-  merge 

Instance Method

# merge

Adds all members of a dictionary to this dictionary.

DriverKitiOSiPadOSmacOS

``` source
bool merge(const OSDictionary * otherDictionary);
```

## Parameters 

`otherDictionary`  

All members of thie dictionary will be added to the array.

## Return Value

True on success, which retains all the added objects, or false on failure which does not retain the objects.

## Discussion

Adds all members of a dictionary to this dictionary. Any keys in the dictionary that exist will be replaced. The dictionary capacity will be grown if necessary.

## See Also

### Creating a Dictionary

withCapacity

Allocates an OSDictionary object with preallocated capacity.

withDictionary

Allocates an OSDictionary object with given members and preallocated capacity.

withObjects

Allocates an OSDictionary object with given members and preallocated capacity.

OSDictionaryCreate

free

flushCollection

Removes and drops references to all members of dictionary.

