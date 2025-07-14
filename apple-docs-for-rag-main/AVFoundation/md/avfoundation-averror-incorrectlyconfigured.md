

- AVFoundation
- AVError
-  incorrectlyConfigured 

Type Property

# incorrectlyConfigured

The system is incorrectly configured for the requested operation.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var incorrectlyConfigured: AVError.Code { get }
```

## Discussion

The system raises this error when you attempt to perform an incorrectly configured operation. For example, HTTP Live Streaming presents only a single video and audio track at a time. If you’re using AVAssetWriter to generate a fragmented MPEG-4 asset for streaming, adding more that one video and audio AVAssetWriterInput to the asset writer generates an error when you start writing.

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

