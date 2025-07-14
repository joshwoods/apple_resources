

- Kernel
- Hardware Families
- FireWire
- IOConfigDirectory
-  getSubdirectories 

# getSubdirectories

``` source
virtual IOReturn getSubdirectories(
 OSIterator *&iterator); 
```

## Parameters 

`iterator`  

on return, set to point to an OSIterator

## Return Value

kIOReturnSuccess if the iterator could be created

## Overview

Creates an iterator over the subdirectories of the directory.

## See Also

### Miscellaneous

getIndexEntry

getIndexKey

getIndexType

getIndexValue

getKeySubdirectories

getKeyType

getKeyValue

update

