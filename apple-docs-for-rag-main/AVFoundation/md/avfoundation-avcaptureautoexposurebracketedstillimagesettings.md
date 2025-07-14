

- AVFoundation
-  AVCaptureAutoExposureBracketedStillImageSettings 

Class

# AVCaptureAutoExposureBracketedStillImageSettings

A configuration for defining bracketed photo captures in terms of bias relative to automatic exposure.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
class AVCaptureAutoExposureBracketedStillImageSettings
```

## Mentioned in 

Capturing a Bracketed Photo Sequence

## Overview

An AVCaptureAutoExposureBracketedStillImageSettings instance defines the exposure target bias setting that should be applied to one image in a bracket. An array of `AVCaptureAutoExposureBracketedStillImageSettings` objects is passed to `captureStillImageBracketAsynchronouslyFromConnection:withSettingsArray:completionHandler:` to specify the bracketing.

The minimum and maximum exposure target bias are properties of the AVCaptureDevice instance supplying data to an AVCaptureStillImageOutput instance. If you wish to leave exposureTargetBias unchanged for this bracketed still image, you may pass the value `AVCaptureExposureTargetBiasCurrent`.

## Topics

### Creating an Auto Exposure Settings Instance

class func autoExposureSettings(exposureTargetBias: Float) -> Self

Creates an `AVCaptureAutoExposureBracketedStillImageSettings` using the specified exposure target bias.

### Getting the Exposure Target Bias

var exposureTargetBias: Float

The exposure bias for the auto exposure bracketed settings

## Relationships

### Inherits From

- AVCaptureBracketedStillImageSettings

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Bracketed Settings Types

class AVCaptureManualExposureBracketedStillImageSettings

A configuration for defining bracketed photo captures in terms of specific exposure and ISO values.

class AVCaptureBracketedStillImageSettings

The abstract superclass for bracketed photo capture settings.

