

- BlockStorageDeviceDriverKit
-  IOUserStorageOptions 

Type Alias

# IOUserStorageOptions

Options that affect the performance of read-write operations.

DriverKit 21.0+

``` source
typedef uint32_t IOUserStorageOptions;
```

## Discussion

Use these options with the DoAsyncReadWrite function.

## Topics

### Storage Options

kIOUserStorageOptionNone

A value that defines no options.

kIOUserStorageOptionForceUnitAccess

An option to use Force Unit Access (FUA).

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

CompleteIO

Indicates that the dext completed an asynchronous read-write call.

