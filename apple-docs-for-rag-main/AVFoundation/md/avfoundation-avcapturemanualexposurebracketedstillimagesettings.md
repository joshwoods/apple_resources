

- AVFoundation
-  AVCaptureManualExposureBracketedStillImageSettings 

Class

# AVCaptureManualExposureBracketedStillImageSettings

A configuration for defining bracketed photo captures in terms of specific exposure and ISO values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
class AVCaptureManualExposureBracketedStillImageSettings
```

## Mentioned in 

Capturing a Bracketed Photo Sequence

## Overview

The `AVCaptureManualExposureBracketedStillImageSettings` class is a concrete subclass of the `AVCaptureBracketedStillImageSettings` class used when bracketing exposure duration and ISO.

An `AVCaptureManualExposureBracketedStillImageSettings` instance defines exposure duration and ISO settings that should be applied to one image in a bracket. An array of `AVCaptureManualExposureBracketedStillImageSettings` objects is passed to `captureStillImageBracketAsynchronouslyFromConnection:withSettingsArray:completionHandler:` to specify the bracketing.

You can query the minimum and maximum duration and ISO properties of the AVCaptureDevice instance supplying data to an AVCaptureStillImageOutput instance. If you wish to leave exposureDuration unchanged for this bracketed still image, you pass the value `AVCaptureExposureDurationCurrent` when creating the instance. To keep the ISO unchanged, you pass `AVCaptureISOCurrent` when creating the instance.

## Topics

### Creating a Manual Bracketed Exposure Settings Instance

class func manualExposureSettings(exposureDuration: CMTime, iso: Float) -> Self

Creates a configuration of still image settings using the specified exposure duration and ISO.

### Getting Manual Exposure Setting Values

var iso: Float

The ISO for the still image.

var exposureDuration: CMTime

The exposure duration for the still image.

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

class AVCaptureAutoExposureBracketedStillImageSettings

A configuration for defining bracketed photo captures in terms of bias relative to automatic exposure.

class AVCaptureBracketedStillImageSettings

The abstract superclass for bracketed photo capture settings.

