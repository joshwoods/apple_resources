

- Kernel
- Hardware Families
- FireWire
- IOConfigDirectory
-  getKeyType 

# getKeyType

``` source
virtual IOReturn getKeyType(
 int key,
 IOConfigKeyType &type); 
```

## Parameters 

`type`  

on return, set to the data type

## Return Value

kIOReturnSuccess if the key exists in the dictionary

## Overview

Gets the data type for the specified key

## See Also

### Miscellaneous

getIndexEntry

getIndexKey

getIndexType

getIndexValue

getKeySubdirectories

getKeyValue

getSubdirectories

update

