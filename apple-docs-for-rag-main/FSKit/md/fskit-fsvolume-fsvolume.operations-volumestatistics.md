

- FSKit
- FSVolume
- FSVolume.Operations
-  volumeStatistics 

Instance Property

# volumeStatistics

A property that provides up-to-date statistics of the volume.

macOS 15.4+

``` source
var volumeStatistics: FSStatFSResult { get }
```

**Required**

## See Also

### Inspecting volume properties

var supportedVolumeCapabilities: FSVolume.SupportedCapabilities

A property that provides the supported capabilities of the volume.

**Required**

class SupportedCapabilities

A type that represents capabillities supported by a volume, such as hard and symbolic links, journaling, and large file sizes.

class FSStatFSResult

A type used to report a volume’s statistics.

