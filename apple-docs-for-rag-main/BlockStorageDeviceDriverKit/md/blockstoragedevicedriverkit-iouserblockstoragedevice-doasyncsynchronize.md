

- BlockStorageDeviceDriverKit
- IOUserBlockStorageDevice
-  DoAsyncSynchronize 

Instance Method

# DoAsyncSynchronize

Forces the hardware buffer to flush data blocks to the media.

DriverKit 21.0+

``` source
kern_return_t DoAsyncSynchronize(uint32_t requestID, uint64_t lba, uint64_t numOfBlocks);
```

## Parameters 

`requestID`  

An opaque identifier. After the dext completes the request, it calls Complete and sends this value as a parameter.

`lba`  

The logical block number of the first block to synchronize.

`numOfBlocks`  

The number of blocks to synchronize.

## Return Value

A value that indicates the synchronize result. kIOReturnSuccess indicates success. For error definitions, see IOKit Constants.

## Discussion

When the synchronize operation completes, the dext calls your Complete method with the results of the operation.

## See Also

### Accessing the Device

DoAsyncUnmap

Sends an asynchronous request to the dext to reclaim storage by unmapping.

BlockRange

A structure that represents a range of blocks.

DoAsyncEjectMedia

Ejects the media.

Complete

Indicates that the dext completed an asynchronous call.

DoAsyncReadWrite

Starts an asynchronous read or write operation.

IOUserStorageOptions

Options that affect the performance of read-write operations.

CompleteIO

Indicates that the dext completed an asynchronous read-write call.

