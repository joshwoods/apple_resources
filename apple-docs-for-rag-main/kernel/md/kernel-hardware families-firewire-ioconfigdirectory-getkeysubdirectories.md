

- Kernel
- Hardware Families
- FireWire
- IOConfigDirectory
-  getKeySubdirectories 

# getKeySubdirectories

``` source
virtual IOReturn getKeySubdirectories(
 intkey,
 OSIterator *&iterator); 
```

## Parameters 

`key`  

type of subdirectory to iterate over

`iterator`  

on return, set to point to an OSIterator

## Return Value

kIOReturnSuccess if the iterator could be created

## Overview

Creates an iterator over subdirectories of a given type of the directory.

## See Also

### Miscellaneous

getIndexEntry

getIndexKey

getIndexType

getIndexValue

getKeyType

getKeyValue

getSubdirectories

update

