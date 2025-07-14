

- Kernel
- Hardware Families
- Mass Storage
- IOBlockStorageDevice
-  doAsyncReadWrite 

# doAsyncReadWrite

Start an asynchronous read or write operation.

``` source
#ifdef __LP64__
 virtual IOReturn doAsyncReadWrite(
 IOMemoryDescriptor *buffer, 
 UInt64 block,
 UInt64 nblks, 
 IOStorageAttributes *attributes, 
 IOStorageCompletion *completion) = 0; 
#else /* !__LP64__ */
virtual IOReturn doAsyncReadWrite(
 IOMemoryDescriptor *buffer, 
 UInt64 block,
 UInt64 nblks, 
 IOStorageAttributes *attributes, 
 IOStorageCompletion *completion); 
#endif 
/* !__LP64__ */
```

## Parameters 

`buffer`  

An IOMemoryDescriptor describing the data-transfer buffer. The data direction is contained in the IOMemoryDescriptor. Responsibility for releasing the descriptor rests with the caller.

`block`  

The starting block number of the data transfer.

`nblks`  

The integral number of blocks to be transferred.

`attributes`  

Attributes of the data transfer. See IOStorageAttributes.

`completion`  

The completion routine to call once the data transfer is complete.

## See Also

### Miscellaneous

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

reportRemovability

Report whether the media is removable or not.

reportWriteProtection

Report whether the media is write-protected or not.

requestIdle

Request that the device enter an idle state.

setWriteCacheState

Sets the write cache state of the device.

