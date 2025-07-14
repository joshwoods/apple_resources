

- BlockStorageDeviceDriverKit
- DeviceParams
-  numOfAddressBits 

Instance Property

# numOfAddressBits

The number of bits used to address blocks on the device.

DriverKit 21.0+

``` source
uint8_t numOfAddressBits;
```

## See Also

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

isUnmapSupported

A Boolean value that indicates whether the device supports unmapping to reclaim storage.

isFUASupported

A Boolean value that indicates whether the device supports forced unit access (FUA).

