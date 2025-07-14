

- AVFoundation
- AVError
-  deviceIsNotAvailableInBackground Deprecated

Type Property

# deviceIsNotAvailableInBackground

You attempted to start a capture session in the background, which isn’t allowed in iOS.

iOS 4.3–9.0DeprecatediPadOS 4.3–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 9.0–9.0Deprecated

``` source
static var deviceIsNotAvailableInBackground: AVError.Code { get }
```

Deprecated

AVCaptureSession no longer produces an AVCaptureSessionRuntimeErrorNotification with this error. See AVCaptureSessionInterruptionReasonVideoDeviceNotAvailableInBackground.

## See Also

### Error Codes

enum Code

An enumeration that defines the errors that framework operations can generate.

static var airPlayControllerRequiresInternet: AVError.Code

The AirPlay controller requires an internet connection to function.

static var airPlayReceiverRequiresInternet: AVError.Code

The AirPlay receiver requires an internet connection to function.

static var airPlayReceiverTemporarilyUnavailable: AVError.Code

An AirPlay receiver is temporarily unavailable.

static var applicationIsNotAuthorized: AVError.Code

The app isn’t authorized to play media.

static var applicationIsNotAuthorizedToUseDevice: AVError.Code

The user denied this app permission to capture media.

static var compositionTrackSegmentsNotContiguous: AVError.Code

The composition can’t add the source media because it contains gaps.

static var contentIsNotAuthorized: AVError.Code

The user isn’t authorized to play the media.

static var contentIsProtected: AVError.Code

The app isn’t authorized to open the media.

static var contentIsUnavailable: AVError.Code

The captured content is unavailable.

static var contentKeyRequestCancelled: AVError.Code

The app canceled a request to retrieve a content key.

static var contentNotUpdated: AVError.Code

The system couldn’t update the captured content.

static var createContentKeyRequestFailed: AVError.Code

The app couldn’t create a content key request.

static var decodeFailed: AVError.Code

The system failed to decode the media.

static var decoderNotFound: AVError.Code

The system can’t find a suitable decoder for the media.

