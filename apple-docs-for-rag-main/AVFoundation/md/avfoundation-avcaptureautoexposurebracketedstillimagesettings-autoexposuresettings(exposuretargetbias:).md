

- AVFoundation
- AVCaptureAutoExposureBracketedStillImageSettings
-  autoExposureSettings(exposureTargetBias:) 

Type Method

# autoExposureSettings(exposureTargetBias:)

Creates an `AVCaptureAutoExposureBracketedStillImageSettings` using the specified exposure target bias.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
class func autoExposureSettings(exposureTargetBias: Float) -> Self
```

## Parameters 

`exposureTargetBias`  

The exposure target bias. Pass `AVCaptureExposureTargetBiasCurrent` to leave the exposureTargetBias unchanged for this image.

## Return Value

An initialized `AVCaptureAutoExposureBracketedStillImageSettings` instance.

