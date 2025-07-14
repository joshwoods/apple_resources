

- BlockStorageDeviceDriverKit
-  BlockRange 

Structure

# BlockRange

A structure that represents a range of blocks.

DriverKit 21.0+

``` source
struct BlockRange;
```

## Discussion

The pure virtual function `_DoAsyncUnmap`, which your dext must implement, takes this type as a parameter that indicates the blocks to unmap.

## Topics

### Accessing Block Range Properties

startBlock

The address of the first block in this range.

numOfBlocks

The number of blocks in this range.

## See Also

### Accessing the Device

DoAsyncUnmap

Sends an asynchronous request to the dext to reclaim storage by unmapping.

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

