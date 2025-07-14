

- AVFoundation
- AVCaptureSession
-  hardwareCost 

Instance Property

# hardwareCost

A value that indicates the percentage of the session’s available hardware budget in use.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 17.0+

``` source
var hardwareCost: Float { get }
```

## Discussion

This property provides a floating-point value from `0.0` to `1.0` that indicates the percentage of a capture session’s hardware that it currently uses. When the value is greater than `1.0`, the capture session can’t run in its current configuration due to hardware constraints. Attempting to start the session while it’s in this state results in a runtime error.

Factors that contribute to the hardware cost include:

- The active formats of the source devices. Some formats use the full sensor (4:3) and others a crop (16:9). Cropped formats require lower hardware bandwidth, and therefore lower the cost.

- The maximum frame rate of the source devices’ active formats. The hardware cost increases when using high frame rates.

- Whether the source devices uses binned formats. Binned formats require substantially less hardware bandwidth, and therefore result in a lower cost.

- The number of sources configured to deliver streaming disparity and depth using AVCaptureDepthDataOutput. The higher the number of cameras configured to produce depth, the higher the cost.

To reduce the hardware cost, consider picking a sensor-cropped or binned activeFormat. You may also use a device input’s videoMinFrameDurationOverride property to artificially limit the maximum frame rate of a source device to a lower value. By doing so, you only pay the hardware cost for the maximum frame rate you intend to use.

Note

AVCaptureSession only computes a nonzero hardware cost when you add multiple AVCaptureVideoDataOutput objects to the session, or an AVCaptureMovieFileOutput instance and one or more instances of AVCaptureVideoDataOutput.

