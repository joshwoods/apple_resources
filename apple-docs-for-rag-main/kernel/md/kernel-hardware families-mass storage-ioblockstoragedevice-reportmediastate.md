

- Kernel
- Hardware Families
- Mass Storage
- IOBlockStorageDevice
-  reportMediaState 

# reportMediaState

Report the device's media state.

``` source
virtual IOReturn reportMediaState(
 bool *mediaPresent,
 bool *changedState = 0) = 0; 
```

## Parameters 

`mediaPresent`  

Pointer to returned media state. True indicates media is present in the device; False indicates no media is present.

## Overview

This method reports whether we have media in the drive or not, and whether the state has changed from the previously reported state.

A result of kIOReturnSuccess is always returned if the test for media is successful, regardless of media presence. The mediaPresent result should be used to determine whether media is present or not. A return other than kIOReturnSuccess indicates that the Transport Driver was unable to interrogate the device. In this error case, the outputs mediaState and changedState will \*not\* be stored.

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

reportRemovability

Report whether the media is removable or not.

reportWriteProtection

Report whether the media is write-protected or not.

requestIdle

Request that the device enter an idle state.

setWriteCacheState

Sets the write cache state of the device.

