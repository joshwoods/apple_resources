

- AVFoundation
- AVCaptureDevice
-  exposurePointOfInterest 

Instance Property

# exposurePointOfInterest

The point of interest for exposure.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
var exposurePointOfInterest: CGPoint { get set }
```

## Discussion

Setting a value for this property doesn’t initiate an exposure rebalancing operation. To set exposure using a point of interest, first set this property’s value, then set the exposureMode property to AVCaptureDevice.ExposureMode.autoExpose or AVCaptureDevice.ExposureMode.continuousAutoExposure.

This property’s CGPoint value uses a coordinate system where `{0,0}` is the top-left of the picture area and `{1,1}` is the bottom-right. This coordinate system is always relative to a landscape device orientation with the home button on the right, regardless of the actual device orientation. You can convert between this coordinate system and view coordinates using AVCaptureVideoPreviewLayer methods.

Before changing the value of this property, you must call lockForConfiguration() to acquire exclusive access to the device’s configuration properties. Otherwise, setting the value of this property raises an exception. When you’re done configuring the device, call unlockForConfiguration() to release the lock and allow other devices to configure the settings.

This property is key-value observable.

## See Also

### Setting an Exposure Point of Interest

var isExposurePointOfInterestSupported: Bool

A Boolean value that indicates whether the device supports a point of interest for exposure.

