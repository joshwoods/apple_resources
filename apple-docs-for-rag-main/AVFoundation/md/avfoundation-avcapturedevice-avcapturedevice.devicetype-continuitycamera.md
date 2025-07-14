

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.DeviceType
-  continuityCamera 

Type Property

# continuityCamera

A Continuity Camera device type.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
static let continuityCamera: AVCaptureDevice.DeviceType
```

## Discussion

You discover devices of this type using an AVCaptureDevice.DiscoverySession of by calling the device’s default(_:for:position:) method.

## See Also

### Cameras

static let builtInWideAngleCamera: AVCaptureDevice.DeviceType

A built-in wide-angle camera device type.

static let builtInUltraWideCamera: AVCaptureDevice.DeviceType

A built-in camera device type with a shorter focal length than a wide-angle camera.

static let builtInTelephotoCamera: AVCaptureDevice.DeviceType

A built-in camera device type with a longer focal length than a wide-angle camera.

static let builtInDualCamera: AVCaptureDevice.DeviceType

A built-in camera device type that consists of a wide-angle and telephoto camera.

static let builtInDualWideCamera: AVCaptureDevice.DeviceType

A built-in camera device type that consists of two cameras of fixed focal length, one ultrawide angle and one wide angle.

static let builtInTripleCamera: AVCaptureDevice.DeviceType

A built-in camera device type that consists of three cameras of fixed focal length, one ultrawide angle, one wide angle, and one telephoto.

static let builtInDuoCamera: AVCaptureDevice.DeviceType

A built-in dual camera device type.

Deprecated

