

- Kernel
- Hardware Families
- FireWire
- IOConfigDirectory
-  getIndexEntry 

# getIndexEntry

``` source
virtual IOReturn getIndexEntry(
 intentry,
 UInt32 &value); 
```

## Parameters 

`entry`  

on return, set to the entry value

`value`  

reference to variable to store the entry's value

## Return Value

kIOReturnSuccess if the index exists in the dictionary

## Overview

Gets the entry at the specified index of the directory, as a raw UInt32.

## See Also

### Miscellaneous

getIndexKey

getIndexType

getIndexValue

getKeySubdirectories

getKeyType

getKeyValue

getSubdirectories

update

