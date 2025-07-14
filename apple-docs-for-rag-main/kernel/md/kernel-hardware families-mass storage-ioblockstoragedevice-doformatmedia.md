

- Kernel
- Hardware Families
- Mass Storage
- IOBlockStorageDevice
-  doFormatMedia 

# doFormatMedia

Format the media to the specified byte capacity.

``` source
virtual IOReturn doFormatMedia(
 UInt64byteCapacity) = 0; 
```

## Parameters 

`byteCapacity`  

The byte capacity to which the device is to be formatted, if possible.

## Overview

The specified byte capacity must be one supported by the device. Supported capacities can be obtained by calling doGetFormatCapacities.

## See Also

### Miscellaneous

doAsyncReadWrite

Start an asynchronous read or write operation.

doEjectMedia

Eject the media.

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

reportRemovability

Report whether the media is removable or not.

reportWriteProtection

Report whether the media is write-protected or not.

requestIdle

Request that the device enter an idle state.

setWriteCacheState

Sets the write cache state of the device.

