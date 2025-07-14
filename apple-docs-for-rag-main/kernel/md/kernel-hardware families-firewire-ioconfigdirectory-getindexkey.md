

- Kernel
- Hardware Families
- FireWire
- IOConfigDirectory
-  getIndexKey 

# getIndexKey

``` source
virtual IOReturn getIndexKey(
 int index,
 int &key); 
```

## Parameters 

`key`  

on return, set to the key

## Return Value

kIOReturnSuccess if the index exists in the dictionary

## Overview

Gets the key for entry at the specified index

## See Also

### Miscellaneous

getIndexEntry

getIndexType

getIndexValue

getKeySubdirectories

getKeyType

getKeyValue

getSubdirectories

update

