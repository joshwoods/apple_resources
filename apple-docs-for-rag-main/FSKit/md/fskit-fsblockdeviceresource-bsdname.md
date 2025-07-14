

- FSKit
- FSBlockDeviceResource
-  bsdName 

Instance Property

# bsdName

The device name of the resource.

macOS 15.4+

``` source
var bsdName: String { get }
```

## See Also

### Accessing resource properties

var isWritable: Bool

A Boolean property that indicates whether the resource can write data to the device.

var blockCount: UInt64

The block count on this resource.

var blockSize: UInt64

The logical block size, the size of data blocks used by the file system.

var physicalBlockSize: UInt64

The sector size of the device.

