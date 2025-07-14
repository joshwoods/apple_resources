

- AVFoundation
- AVCaptureManualExposureBracketedStillImageSettings
-  manualExposureSettings(exposureDuration:iso:) 

Type Method

# manualExposureSettings(exposureDuration:iso:)

Creates a configuration of still image settings using the specified exposure duration and ISO.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
class func manualExposureSettings(
    exposureDuration duration: CMTime,
    iso ISO: Float
) -> Self
```

## Parameters 

`duration`  

The exposure duration in seconds. Pass `AVCaptureExposureDurationCurrent` to leave the duration unchanged for this bracketed image.

`ISO`  

The film speed in the ISO format. Pass `AVCaptureISOCurrent` to leave the ISO unchanged for this bracketed image.

## Return Value

An initialized `AVCaptureManualExposureBracketedStillImageSettings` instance.

