

- Application Services
- ColorSync Manager
-  CMDeviceInfo 

Structure

# CMDeviceInfo

macOS 10.0+

``` source
struct CMDeviceInfo
```

## Topics

### Initializers

init()

init(dataVersion: UInt32, deviceClass: CMDeviceClass, deviceID: UInt32, deviceScope: CMDeviceScope, deviceState: UInt32, defaultProfileID: UInt32, deviceName: UnsafeMutablePointer&lt;Unmanaged&lt;CFDictionary>?>!, profileCount: UInt32, reserved: UInt32)

### Instance Properties

var dataVersion: UInt32

var defaultProfileID: UInt32

var deviceClass: CMDeviceClass

var deviceID: UInt32

var deviceName: UnsafeMutablePointer&lt;Unmanaged&lt;CFDictionary>?>!

See the CFDictionary documentation for a description of the `CFDictionaryRef` data type.

var deviceScope: CMDeviceScope

var deviceState: UInt32

var profileCount: UInt32

var reserved: UInt32

