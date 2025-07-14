

- AVFoundation
-  AVCaptureStillImageOutput Deprecated

Class

# AVCaptureStillImageOutput

A capture output for capturing still photos.

iOS 4.0–10.0DeprecatediPadOS 4.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.7–10.15Deprecated

``` source
class AVCaptureStillImageOutput
```

Deprecated

Use AVCapturePhotoOutput instead.

## Topics

### Capturing an Image

func captureStillImageAsynchronously(from: AVCaptureConnection, completionHandler: (CMSampleBuffer?, (any Error)?) -> Void)

Initiates a still image capture and returns immediately.

var isCapturingStillImage: Bool

Indicates whether a still image is being captured.

### Getting and Setting Image Stabilization Settings

var isStillImageStabilizationActive: Bool

Indicates whether still image stabilization is in use for the current capture.

var automaticallyEnablesStillImageStabilizationWhenAvailable: Bool

A Boolean value that indicates whether still image stabilization should be automatically enabled.

var isStillImageStabilizationSupported: Bool

A Boolean value that indicates whether the still image currently being captured supports still image stabilization.

### Configuring Image Settings

var isHighResolutionStillImageOutputEnabled: Bool

A Boolean value that indicates whether the receiver should emit still images at the highest resolution supported by its source `AVCaptureDevice` objects `activeFormat` property.

var availableImageDataCVPixelFormatTypes: [NSNumber]

The supported image pixel formats that can be specified as output settings.

var availableImageDataCodecTypes: [AVVideoCodecType]

The supported image codec formats that can be specified as output settings.

var outputSettings: [String : Any]

The compression settings for the output.

Video settings

Configure video processing settings using standard key and value constants.

### Image Format Conversion

class func jpegStillImageNSDataRepresentation(CMSampleBuffer) -> Data?

Returns an `NSData` representation of a still image data and metadata attachments in a JPEG sample buffer.

### Still Image Bracketed Capture

func captureStillImageBracketAsynchronously(from: AVCaptureConnection, withSettingsArray: [AVCaptureBracketedStillImageSettings], completionHandler: (CMSampleBuffer?, AVCaptureBracketedStillImageSettings?, (any Error)?) -> Void)

Captures a still image bracket.

var maxBracketedCaptureStillImageCount: Int

Specifies the maximum number of still images that may be taken in a single bracket.

func prepareToCaptureStillImageBracket(from: AVCaptureConnection, withSettingsArray: [AVCaptureBracketedStillImageSettings], completionHandler: (Bool, (any Error)?) -> Void)

Allows the receiver to prepare resources in advance of capturing a still image bracket.

var isLensStabilizationDuringBracketedCaptureSupported: Bool

A Boolean value that indicates whether the capture output supports lens stabilization across the duration of a bracketed capture.

var isLensStabilizationDuringBracketedCaptureEnabled: Bool

A Boolean value that specifies whether to stabilize the lens across the duration of a bracketed capture.

### Creating Still Image Output

init()

Creates new still image output.

## Relationships

### Inherits From

- AVCaptureOutput

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Photo capture

Capturing consistent color images

Add the power of a photography studio and lighting rig to your app with the new Constant Color API.

Capturing Still and Live Photos

Configure and capture single or multiple still images, Live Photos, and other forms of photography.

Capturing Photos in RAW and Apple ProRAW Formats

Support professional photography workflows by enabling minimally processed image capture in your camera app.

Supporting Continuity Camera in Your Mac App

Incorporate scanned documents and pictures from a user’s iPhone, iPad, or iPod touch into your Mac app using Continuity Camera.

class AVCapturePhoto

A container for image data from a photo capture output.

class AVCaptureDeferredPhotoProxy

A lightly-processed photo with data that the system may use to process and fetch a higher-resolution asset at a later time.

class AVCapturePhotoOutput

A capture output for still image, Live Photos, and other photography workflows.

protocol AVCapturePhotoCaptureDelegate

Methods for monitoring progress and receiving results from a photo capture output.

class AVCapturePhotoOutputReadinessCoordinator

An object that monitors changes to a photo output’s capture readiness.

protocol AVCapturePhotoOutputReadinessCoordinatorDelegate

A delegate protocol to receive updates about a photo output’s capture readiness.

