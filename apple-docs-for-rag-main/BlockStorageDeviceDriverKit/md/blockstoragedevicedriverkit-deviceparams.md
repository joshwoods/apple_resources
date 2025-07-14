

- BlockStorageDeviceDriverKit
-  DeviceParams 

Structure

# DeviceParams

A structure that represents hardware-specific properties of the block storage device.

DriverKit 21.0+

``` source
struct DeviceParams;
```

## Discussion

Implement the GetDeviceParams method to provide the framework with the device-specific properties indicated by this structure.

## Topics

### Accessing Device Parameters

numOfBlocks

The number of blocks on the device.

blockSize

The size of a block on the device.

maxIOSize

The maximum amount of data per I/O call.

numOfOutstandingIOs

The upper limit to the number of requests sent to the device.

maxNumOfUnmapRegions

The maximum number of regions supported by an unmap call.

minSegmentAlignment

The minimum alignment of the data buffer sent to read-write calls.

numOfAddressBits

The number of bits used to address blocks on the device.

isUnmapSupported

A Boolean value that indicates whether the device supports unmapping to reclaim storage.

isFUASupported

A Boolean value that indicates whether the device supports forced unit access (FUA).

## See Also

### Reporting Device Metadata

GetVendorString

Gets a string that identifies the vendor in response to a call from the framework.

GetProductString

Gets a string that identifies the product in response to a call from the framework.

GetRevisionString

Gets a string that identifies the current revision in response to a call from the framework.

GetAdditionalInfoString

Gets a string that provides additional information in response to a call from the framework.

DeviceString

A type that represents a string of character data from the device.

GetDeviceParams

Gets device parameters in response to a call from the framework.

