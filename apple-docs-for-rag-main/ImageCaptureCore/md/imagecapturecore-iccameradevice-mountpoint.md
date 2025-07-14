

- ImageCaptureCore
- ICCameraDevice
-  mountPoint 

Instance Property

# mountPoint

The file system mount point for a camera using the mass storage transport type.

macOS 10.4+

``` source
var mountPoint: String? { get }
```

## Discussion

This property is set for cameras whose transportType is transportTypeMassStorage.

