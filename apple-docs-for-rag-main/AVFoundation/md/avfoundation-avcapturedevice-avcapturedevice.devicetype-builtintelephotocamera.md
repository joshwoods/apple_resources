

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.DeviceType
-  builtInTelephotoCamera 

Type Property

# builtInTelephotoCamera

A built-in camera device type with a longer focal length than a wide-angle camera.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
static let builtInTelephotoCamera: AVCaptureDevice.DeviceType
```

## Discussion

You can only discover this device type using an AVCaptureDevice.DiscoverySession.

## See Also

### Cameras

static let builtInWideAngleCamera: AVCaptureDevice.DeviceType

A built-in wide-angle camera device type.

static let builtInUltraWideCamera: AVCaptureDevice.DeviceType

A built-in camera device type with a shorter focal length than a wide-angle camera.

static let builtInDualCamera: AVCaptureDevice.DeviceType

A built-in camera device type that consists of a wide-angle and telephoto camera.

static let builtInDualWideCamera: AVCaptureDevice.DeviceType

A built-in camera device type that consists of two cameras of fixed focal length, one ultrawide angle and one wide angle.

static let builtInTripleCamera: AVCaptureDevice.DeviceType

A built-in camera device type that consists of three cameras of fixed focal length, one ultrawide angle, one wide angle, and one telephoto.

static let continuityCamera: AVCaptureDevice.DeviceType

A Continuity Camera device type.

static let builtInDuoCamera: AVCaptureDevice.DeviceType

A built-in dual camera device type.

Deprecated

