

- AVFoundation
- AVCaptureDeviceInput
-  unifiedAutoExposureDefaultsEnabled 

Instance Property

# unifiedAutoExposureDefaultsEnabled

A Boolean value that indicates whether the input enables unified auto-exposure defaults.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var unifiedAutoExposureDefaultsEnabled: Bool { get set }
```

## Discussion

You may set the value of a capture device’s activeFormat in two ways:

1.  Set it directly using one of the formats in the device’s formats property.

2.  The capture session sets it on your behalf when you set its sessionPreset property.

Depending on the device and format, you may configure the default auto exposure behavior differently when you use one method or the other, resulting in non-uniform auto exposure behavior. Auto exposure defaults include minFrameRate, maxFrameRate, and maxExposureDuration. You can set this property to true to ensure that the system applies consistent default behaviors to the device regardless of the way you set the active format.

The default value is false.

Note

Manually setting the device’s minFrameRate, maxFrameRate, or maxExposureDuration overrides the device defaults, even if you set this property to true.

## See Also

### Configuring video properties

var videoMinFrameDurationOverride: CMTime

A time value that acts as a modifier to a capture device’s active video minimum frame duration.

