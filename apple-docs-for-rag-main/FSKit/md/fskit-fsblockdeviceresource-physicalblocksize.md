

- FSKit
- FSBlockDeviceResource
-  physicalBlockSize 

Instance Property

# physicalBlockSize

The sector size of the device.

macOS 15.4+

``` source
var physicalBlockSize: UInt64 { get }
```

## Discussion

This is equivalent to the `DKIOCGETPHYSICALBLOCKSIZE` device parameter.

## See Also

### Accessing resource properties

var bsdName: String

The device name of the resource.

var isWritable: Bool

A Boolean property that indicates whether the resource can write data to the device.

var blockCount: UInt64

The block count on this resource.

var blockSize: UInt64

The logical block size, the size of data blocks used by the file system.

