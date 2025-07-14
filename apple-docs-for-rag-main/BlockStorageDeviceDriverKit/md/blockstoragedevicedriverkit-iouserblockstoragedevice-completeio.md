

- BlockStorageDeviceDriverKit
- IOUserBlockStorageDevice
-  CompleteIO 

Instance Method

# CompleteIO

Indicates that the dext completed an asynchronous read-write call.

DriverKit 21.0+

``` source
void CompleteIO(uint32_t requestID, uint64_t bytesTransferred, kern_return_t IOStatus);
```

## Parameters 

`requestID`  

An opaque identifier, originally provided in the corresponding DoAsyncReadWrite call.

`bytesTransferred`  

The number of bytes transferred.

`IOStatus`  

The status of the request.

## Discussion

The dext calls this method to indicate completion of an asynchronous read-write call. Use the `requestID` parameter to determine which DoAsyncReadWrite call resulted in this callback.

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

DoAsyncReadWrite

Starts an asynchronous read or write operation.

IOUserStorageOptions

Options that affect the performance of read-write operations.

