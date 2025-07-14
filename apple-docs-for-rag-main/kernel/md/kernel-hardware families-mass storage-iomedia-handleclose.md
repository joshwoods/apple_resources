

- Kernel
- Hardware Families
- Mass Storage
- IOMedia
-  handleClose 

# handleClose

``` source
virtual void handleClose(
 IOService *client,
 IOOptionBitsoptions); 
```

## Parameters 

`client`  

Client requesting the close.

`options`  

Options for the close. Set to zero.

## Overview

The handleClose method closes the client's access to this object.

This implementation replaces the IOService definition of handleClose().

## See Also

### Miscellaneous

copyPhysicalExtent

getAttributes

getBase

getContent

getContentHint

getPreferredBlockSize

getSize

handleIsOpen

handleOpen

init

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

