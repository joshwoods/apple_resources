

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.DeviceType
-  builtInDualCamera 

Type Property

# builtInDualCamera

A built-in camera device type that consists of a wide-angle and telephoto camera.

iOS 10.2+iPadOS 10.2+Mac Catalyst 14.0+tvOS 17.0+

``` source
static let builtInDualCamera: AVCaptureDevice.DeviceType
```

## Mentioned in 

Capturing Photos with Depth

## Discussion

This device type supports the following features:

- Automatic switching from one camera to the other when the zoom factor, light level, and focus position allow.

- Higher-quality zoom for still captures by fusing images from both cameras.

- Depth data delivery by measuring the disparity of matched features between the wide and telephoto cameras.

- Delivery of photos from constituent devices (wide and telephoto cameras) from a single photo capture request.

It doesn’t support the features below:

- Setting a AVCaptureDevice.ExposureMode.custom exposure mode or manual exposure bracketing.

- Locking focus with a lens position to a value other than currentLensPosition.

- Locking automatic white balance with device white balance gains other than currentWhiteBalanceGains.

Even when locked, exposure duration, ISO, aperture, white balance gains, or lens position may change when the device switches from one camera to the other. The overall exposure, white balance, and focus position however should be consistent.

You can only retrieve devices of this type using an AVCaptureDevice.DiscoverySession or by calling default(_:for:position:).

## See Also

### Cameras

static let builtInWideAngleCamera: AVCaptureDevice.DeviceType

A built-in wide-angle camera device type.

static let builtInUltraWideCamera: AVCaptureDevice.DeviceType

A built-in camera device type with a shorter focal length than a wide-angle camera.

static let builtInTelephotoCamera: AVCaptureDevice.DeviceType

A built-in camera device type with a longer focal length than a wide-angle camera.

static let builtInDualWideCamera: AVCaptureDevice.DeviceType

A built-in camera device type that consists of two cameras of fixed focal length, one ultrawide angle and one wide angle.

static let builtInTripleCamera: AVCaptureDevice.DeviceType

A built-in camera device type that consists of three cameras of fixed focal length, one ultrawide angle, one wide angle, and one telephoto.

static let continuityCamera: AVCaptureDevice.DeviceType

A Continuity Camera device type.

static let builtInDuoCamera: AVCaptureDevice.DeviceType

A built-in dual camera device type.

Deprecated

