

- BlockStorageDeviceDriverKit
- IOUserBlockStorageDevice
-  Complete 

Instance Method

# Complete

Indicates that the dext completed an asynchronous call.

DriverKit 21.0+

``` source
void Complete(uint32_t requestID, kern_return_t status);
```

## Parameters 

`requestID`  

An opaque identifier, originally provided in the corresponding `DoAsync…` call.

`status`  

The status of the request.

## Discussion

The dext calls this method to indicate completion of an asynchronous call to methods like DoAsyncUnmap, DoAsyncSynchronize, or DoAsyncEjectMedia. Use the `requestID` parameter to determine which call resulted in this callback.

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

DoAsyncReadWrite

Starts an asynchronous read or write operation.

IOUserStorageOptions

Options that affect the performance of read-write operations.

CompleteIO

Indicates that the dext completed an asynchronous read-write call.

