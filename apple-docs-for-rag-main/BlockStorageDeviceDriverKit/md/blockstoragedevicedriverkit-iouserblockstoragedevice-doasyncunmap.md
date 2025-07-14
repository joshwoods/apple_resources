

- BlockStorageDeviceDriverKit
- IOUserBlockStorageDevice
-  DoAsyncUnmap 

Instance Method

# DoAsyncUnmap

Sends an asynchronous request to the dext to reclaim storage by unmapping.

DriverKit 21.0+

``` source
kern_return_t DoAsyncUnmap(uint32_t requestID, IOMemoryDescriptor * buffer, uint32_t numOfRanges);
```

## Parameters 

`requestID`  

An opaque identifier. After the dext completes the request, it calls Complete and sends this value as a parameter.

`buffer`  

A memory buffer containing the block ranges to unmap.

`numOfRanges`  

The number of ranges in `buffer`.

## Return Value

A value that indicates the unmap result. kIOReturnSuccess indicates success. For error definitions, see IOKit Constants.

## Discussion

When the unmap operation completes, the dext calls your Complete method with the results of the operation.

## See Also

### Accessing the Device

BlockRange

A structure that represents a range of blocks.

DoAsyncSynchronize

Forces the hardware buffer to flush data blocks to the media.

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

