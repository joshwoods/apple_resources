

- Kernel
- Hardware Families
- Mass Storage
- IOBlockStorageDevice
-  reportRemovability 

# reportRemovability

Report whether the media is removable or not.

``` source
virtual IOReturn reportRemovability(
 bool *isRemovable) = 0; 
```

## Parameters 

`isRemovable`  

Pointer to returned result. True indicates that the media is removable; False indicates the media is not removable.

## Overview

This method reports whether the media is removable, but it does not provide detailed information regarding software eject or lock/unlock capability.

## See Also

### Miscellaneous

doAsyncReadWrite

Start an asynchronous read or write operation.

doEjectMedia

Eject the media.

doFormatMedia

Format the media to the specified byte capacity.

doGetFormatCapacities

Return the allowable formatting byte capacities.

doSynchronizeCache

Force data blocks in the hardware's buffer to be flushed to the media.

doUnmap

Delete unused data blocks from the media.

getAdditionalDeviceInfoString

Return additional informational string for the device.

getProductString

Return Product Name string for the device.

getRevisionString

Return Product Revision string for the device.

getVendorString

Return Vendor Name string for the device.

getWriteCacheState

Reports the current write cache state of the device.

init

reportBlockSize

Report the block size for the device, in bytes.

reportEjectability

Report if the media is ejectable under software control.

reportMaxValidBlock

Report the highest valid block for the device.

reportMediaState

Report the device's media state.

reportWriteProtection

Report whether the media is write-protected or not.

requestIdle

Request that the device enter an idle state.

setWriteCacheState

Sets the write cache state of the device.

