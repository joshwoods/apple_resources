

- AVFoundation
- AVError
-  airPlayReceiverRequiresInternet 

Type Property

# airPlayReceiverRequiresInternet

The AirPlay receiver requires an internet connection to function.

iOS 8.3+iPadOS 8.3+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.3+

``` source
static var airPlayReceiverRequiresInternet: AVError.Code { get }
```

## See Also

### Error Codes

enum Code

An enumeration that defines the errors that framework operations can generate.

static var airPlayControllerRequiresInternet: AVError.Code

The AirPlay controller requires an internet connection to function.

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

static var decoderTemporarilyUnavailable: AVError.Code

A suitable decoder for the media is temporarily available.

