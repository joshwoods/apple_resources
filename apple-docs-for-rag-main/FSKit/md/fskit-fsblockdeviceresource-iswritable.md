

- FSKit
- FSBlockDeviceResource
-  isWritable 

Instance Property

# isWritable

A Boolean property that indicates whether the resource can write data to the device.

macOS 15.4+

``` source
var isWritable: Bool { get }
```

## See Also

### Accessing resource properties

var bsdName: String

The device name of the resource.

var blockCount: UInt64

The block count on this resource.

var blockSize: UInt64

The logical block size, the size of data blocks used by the file system.

var physicalBlockSize: UInt64

The sector size of the device.

