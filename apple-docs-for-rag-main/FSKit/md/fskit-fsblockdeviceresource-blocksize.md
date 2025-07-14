

- FSKit
- FSBlockDeviceResource
-  blockSize 

Instance Property

# blockSize

The logical block size, the size of data blocks used by the file system.

macOS 15.4+

``` source
var blockSize: UInt64 { get }
```

## Discussion

This is equivalent to the `DKIOCGETBLOCKSIZE` device parameter.

## See Also

### Accessing resource properties

var bsdName: String

The device name of the resource.

var isWritable: Bool

A Boolean property that indicates whether the resource can write data to the device.

var blockCount: UInt64

The block count on this resource.

var physicalBlockSize: UInt64

The sector size of the device.

