

- FSKit
- FSVolume
- FSVolume.Operations
-  supportedVolumeCapabilities 

Instance Property

# supportedVolumeCapabilities

A property that provides the supported capabilities of the volume.

macOS 15.4+

``` source
var supportedVolumeCapabilities: FSVolume.SupportedCapabilities { get }
```

**Required**

## See Also

### Inspecting volume properties

class SupportedCapabilities

A type that represents capabillities supported by a volume, such as hard and symbolic links, journaling, and large file sizes.

var volumeStatistics: FSStatFSResult

A property that provides up-to-date statistics of the volume.

**Required**

class FSStatFSResult

A type used to report a volume’s statistics.

