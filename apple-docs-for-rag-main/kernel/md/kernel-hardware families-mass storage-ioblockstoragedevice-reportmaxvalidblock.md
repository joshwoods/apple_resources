

- Kernel
- Hardware Families
- Mass Storage
- IOBlockStorageDevice
-  reportMaxValidBlock 

# reportMaxValidBlock

Report the highest valid block for the device.

``` source
virtual IOReturn reportMaxValidBlock(
 UInt64 *maxBlock) = 0; 
```

## Parameters 

`maxBlock`  

Pointer to returned result

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

