

- Kernel
- Hardware Families
- FireWire
- IOConfigDirectory
-  getIndexType 

# getIndexType

``` source
virtual IOReturn getIndexType(
 int index,
 IOConfigKeyType &type); 
```

## Parameters 

`type`  

on return, set to the data type

## Return Value

kIOReturnSuccess if the index exists in the dictionary

## Overview

Gets the data type for entry at the specified index

## See Also

### Miscellaneous

getIndexEntry

getIndexKey

getIndexValue

getKeySubdirectories

getKeyType

getKeyValue

getSubdirectories

update

