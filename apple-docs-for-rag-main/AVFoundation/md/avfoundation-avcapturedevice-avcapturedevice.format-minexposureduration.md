

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.Format
-  minExposureDuration 

Instance Property

# minExposureDuration

A time value that indicates the minimum supported exposure duration.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var minExposureDuration: CMTime { get }
```

## See Also

### Determining Exposure Support

var systemRecommendedExposureBiasRange: ClosedRange&lt;Float>?

The system’s recommended exposure bias range for this device format.

var minISO: Float

A floating-point number that indicates the minimum supported exposure ISO value.

var maxISO: Float

A floating-point number that indicates the maximum supported exposure ISO value.

var maxExposureDuration: CMTime

A time value that indicates the maximum supported exposure duration.

