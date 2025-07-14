

- Kernel
- Hardware Families
- Mass Storage
- IOBlockStorageDevice
-  doGetFormatCapacities 

# doGetFormatCapacities

Return the allowable formatting byte capacities.

``` source
virtual UInt32 doGetFormatCapacities(
 UInt64 *capacities, 
 UInt32capacitiesMaxCount) const = 0; 
```

## Parameters 

`capacities`  

Pointer for returning the list of capacities.

`capacitiesMaxCount`  

The number of capacity values returned in "capacities," or if no buffer is given, the total number of capacity values available.

## Overview

This function returns the supported byte capacities for the device.

## See Also

### Miscellaneous

doAsyncReadWrite

Start an asynchronous read or write operation.

doEjectMedia

Eject the media.

doFormatMedia

Format the media to the specified byte capacity.

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

reportRemovability

Report whether the media is removable or not.

reportWriteProtection

Report whether the media is write-protected or not.

requestIdle

Request that the device enter an idle state.

setWriteCacheState

Sets the write cache state of the device.

