

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.Format
-  systemRecommendedExposureBiasRange 

Instance Property

# systemRecommendedExposureBiasRange

The system’s recommended exposure bias range for this device format.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
@nonobjc
var systemRecommendedExposureBiasRange: ClosedRange? { get }
```

## Discussion

Use this value to create a slider in your app’s user interface that controls a device’s exposure bias within a system-recommended range. When a recommendation isn’t available, this property returns `nil`.

Note

The framework uses this value to define the range of an AVCaptureSystemExposureBiasSlider control.

## See Also

### Determining Exposure Support

var minISO: Float

A floating-point number that indicates the minimum supported exposure ISO value.

var maxISO: Float

A floating-point number that indicates the maximum supported exposure ISO value.

var minExposureDuration: CMTime

A time value that indicates the minimum supported exposure duration.

var maxExposureDuration: CMTime

A time value that indicates the maximum supported exposure duration.

