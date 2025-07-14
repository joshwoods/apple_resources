

- AVFoundation
-  AVCapturePhotoBracketSettings 

Class

# AVCapturePhotoBracketSettings

A specification of the features and settings to use for a photo capture request that captures multiple images with varied settings.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
class AVCapturePhotoBracketSettings
```

## Mentioned in 

Capturing a Bracketed Photo Sequence

## Overview

To take a bracketed capture, you create and configure an AVCapturePhotoBracketSettings object, using AVCaptureBracketedStillImageSettings objects to describe the individual captures in the bracket, and then pass it to the AVCapturePhotoOutput capturePhoto(with:delegate:) method.

To request a bracketed capture, follow these steps:

1.  Create an array of AVCaptureBracketedStillImageSettings objects describing the number of images to capture in the bracket and the variations on capture settings between them.

2.  Create a bracketed photo settings object with the init(rawPixelFormatType:processedFormat:bracketedSettings:) initializer, passing the array of bracketed still image settings, along with the processed format (such as JPEG) or RAW format to capture images in.

3.  Configure other settings to share across all images in the bracket, such as the isLensStabilizationEnabled property and certain inherited properties.

Important

Bracketed capture supports only the isHighResolutionPhotoEnabled and previewPhotoFormat settings defined by the AVCapturePhotoSettings superclass. Bracketed capture does not support flash, auto stabilization, or Live Photos—attempting to set any of the corresponding properties raises an exception.

4.  Initiate capture by passing the bracketed photo settings object to your photo output’s capturePhoto(with:delegate:) method, along with a delegate object to receive messages about the progress and results of the capture.

Tip

Capturing a multiple-image bracket may require allocation of additional resources. See the setPreparedPhotoSettingsArray(_:completionHandler:) method.

5.  The photo output calls your delegate’s photoOutput(_:didFinishProcessingPhoto:previewPhoto:resolvedSettings:bracketSettings:error:) or photoOutput(_:didFinishProcessingRawPhoto:previewPhoto:resolvedSettings:bracketSettings:error:) methods many times corresponding to the number of captures in the bracket. Each call provides the AVCaptureBracketedStillImageSettings object indicating which capture in the bracket the captured image corresponds to.

The following code example illustrates capturing a bracket of three RAW images with varying exposure value settings.

Listing 1. Capturing a Multi-Exposure Bracket

- Swift
- Objective-C

```
func captureRAWAutoExposureBracket() {
    guard myCapturePhotoOutput.maxBracketedCapturePhotoCount >= 3 else { return }

    // Specify a 3-shot bracket, where exposure compensation varies between each shot.
    let makeSettings = AVCaptureAutoExposureBracketedStillImageSettings.autoExposureSettingsWithExposureTargetBias
    let bracketedStillImageSettings = [-2, 0, 2].map { makeSettings(Float($0))! }
    let rawFormat = myCapturePhotoOutput.availableRawPhotoCVPixelFormatTypes.first!.unsignedIntValue as OSType

    let settings = AVCapturePhotoBracketSettings(format: nil, rawPixelFormatType: rawFormat, bracketedSettings: bracketedStillImageSettings)
    settings.lensStabilizationEnabled = myCapturePhotoOutput.lensStabilizationDuringBracketedCaptureSupported

    myCapturePhotoOutput.capturePhotoWithSettings(settings, delegate: self)
    // Three RAW photos will be delivered.
}
```

```
- (void)captureRAWAutoExposureBracket {
    if ( myCapturePhotoOutput.maxBracketedCapturePhotoCount 

## Topics

### Creating a Bracket Settings Object

convenience init(rawPixelFormatType: OSType, rawFileType: AVFileType?, processedFormat: [String : Any]?, processedFileType: AVFileType?, bracketedSettings: [AVCaptureBracketedStillImageSettings])

Creates a photo settings object for capture in both RAW format and a processed format.

convenience init(rawPixelFormatType: OSType, processedFormat: [String : Any]?, bracketedSettings: [AVCaptureBracketedStillImageSettings])

Creates a photo settings object for the specified bracket of captures, in the specified formats.

### Working with Bracketed Settings

var bracketedSettings: [AVCaptureBracketedStillImageSettings]

An array describing the number of and settings for images to produce in a bracketed capture.

var isLensStabilizationEnabled: Bool

A Boolean value that specifies whether to stabilize the lens for the duration of the bracketed capture.

### Bracketed Settings Types

class AVCaptureAutoExposureBracketedStillImageSettings

A configuration for defining bracketed photo captures in terms of bias relative to automatic exposure.

class AVCaptureManualExposureBracketedStillImageSettings

A configuration for defining bracketed photo captures in terms of specific exposure and ISO values.

class AVCaptureBracketedStillImageSettings

The abstract superclass for bracketed photo capture settings.

## Relationships

### Inherits From

- AVCapturePhotoSettings

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Photo settings

class AVCapturePhotoSettings

A specification of the features and settings to use for a single photo capture request.

class AVCaptureResolvedPhotoSettings

A description of the features and settings in use for an in-progress or complete photo capture request.

