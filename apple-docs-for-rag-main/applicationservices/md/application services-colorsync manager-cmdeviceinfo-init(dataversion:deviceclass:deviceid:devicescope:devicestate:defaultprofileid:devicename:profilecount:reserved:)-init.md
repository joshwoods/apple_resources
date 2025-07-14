

- Application Services
- ColorSync Manager
- CMDeviceInfo
-  init(dataVersion:deviceClass:deviceID:deviceScope:deviceState:defaultProfileID:deviceName:profileCount:reserved:) 

Initializer

# init(dataVersion:deviceClass:deviceID:deviceScope:deviceState:defaultProfileID:deviceName:profileCount:reserved:)

macOS 10.9+Xcode 9.0+

``` source
init(
    dataVersion: UInt32,
    deviceClass: CMDeviceClass,
    deviceID: UInt32,
    deviceScope: CMDeviceScope,
    deviceState: UInt32,
    defaultProfileID: UInt32,
    deviceName: UnsafeMutablePointer?>!,
    profileCount: UInt32,
    reserved: UInt32
)
```

