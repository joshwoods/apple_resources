

- Kernel
- Hardware Families
- Mass Storage
- IOMedia
-  init 

# init

``` source
virtual bool init(
 UInt64 base, 
 UInt64 size, 
 UInt64 preferredBlockSize, 
 IOMediaAttributeMask attributes, 
 bool isWhole, 
 bool isWritable, 
 const char *contentHint = 0, 
 OSDictionary *properties = 0); 
```

## Parameters 

`base`  

Media offset, in bytes.

`size`  

Media size, in bytes.

`preferredBlockSize`  

Natural block size, in bytes.

`attributes`  

Media attributes, such as ejectability and removability. See IOMediaAttributeMask.

`isWhole`  

Indicates whether the media represents the whole disk.

`isWritable`  

Indicates whether the media is writable.

`contentHint`  

Hint of media's contents (optional). See getContentHint().

`properties`  

Substitute property table for this object (optional).

## Return Value

Returns true on success, false otherwise.

## Overview

Initialize this object's minimal state.

## See Also

### Miscellaneous

copyPhysicalExtent

getAttributes

getBase

getContent

getContentHint

getPreferredBlockSize

getSize

handleClose

handleIsOpen

handleOpen

isEjectable

isFormatted

isWhole

isWritable

lockPhysicalExtents

read

synchronizeCache

unlockPhysicalExtents

unmap

write

