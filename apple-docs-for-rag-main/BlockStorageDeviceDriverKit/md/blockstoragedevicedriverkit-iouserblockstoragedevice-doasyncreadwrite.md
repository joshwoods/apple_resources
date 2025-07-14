

- BlockStorageDeviceDriverKit
- IOUserBlockStorageDevice
-  DoAsyncReadWrite 

Instance Method

# DoAsyncReadWrite

Starts an asynchronous read or write operation.

DriverKit 21.0+

``` source
kern_return_t DoAsyncReadWrite(bool isRead, uint32_t requestID, uint64_t dmaAddr, uint64_t size, uint64_t lba, uint64_t numOfBlocks, IOUserStorageOptions options);
```

## Parameters 

`requestID`  

An opaque identifier. After the dext completes the request, it calls CompleteIO and sends this value as a parameter.

`dmaAddr`  

The DMA address of the data buffer.

`size`  

The size of the data buffer.

`lba`  

The start logical block number.

`numOfBlocks`  

The number of blocks to read or write.

`options`  

Data transfer options. These can be any combination of `kIOUserStorage…` values (defined in IOUserStorageOptions) combined together with the logical `OR` operator.

## Return Value

A value that indicates the result of the read/write operation. kIOReturnSuccess indicates success. For error definitions, see IOKit Constants.

## Discussion

When the read or write operation completes, the dext calls your CompleteIO method with the results of the operation.

## See Also

### Accessing the Device

DoAsyncUnmap

Sends an asynchronous request to the dext to reclaim storage by unmapping.

BlockRange

A structure that represents a range of blocks.

DoAsyncSynchronize

Forces the hardware buffer to flush data blocks to the media.

DoAsyncEjectMedia

Ejects the media.

Complete

Indicates that the dext completed an asynchronous call.

IOUserStorageOptions

Options that affect the performance of read-write operations.

CompleteIO

Indicates that the dext completed an asynchronous read-write call.

