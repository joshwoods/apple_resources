

- AVFoundation
- AVError
-  AVError.Code 

Enumeration

# AVError.Code

An enumeration that defines the errors that framework operations can generate.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum Code
```

## Topics

### Error Codes

case airPlayControllerRequiresInternet

The AirPlay controller requires an internet connection to function.

case airPlayReceiverRequiresInternet

The AirPlay receiver requires an internet connection to function.

case airPlayReceiverTemporarilyUnavailable

An AirPlay receiver is temporarily unavailable.

case applicationIsNotAuthorized

The app isn’t authorized to play media.

case applicationIsNotAuthorizedToUseDevice

The user denied this app permission to capture media.

case compositionTrackSegmentsNotContiguous

The composition can’t add the source media because it contains gaps.

case contentIsNotAuthorized

The user isn’t authorized to play the media.

case contentIsProtected

The app isn’t authorized to open the media.

case contentIsUnavailable

The captured content is unavailable.

case contentKeyRequestCancelled

The app canceled a request to retrieve a content key.

case contentNotUpdated

The system couldn’t update the captured content.

case createContentKeyRequestFailed

The app couldn’t create a content key request.

case decodeFailed

The system failed to decode the media.

case decoderNotFound

The system can’t find a suitable decoder for the media.

case decoderTemporarilyUnavailable

A suitable decoder for the media is temporarily available.

case deviceAlreadyUsedByAnotherSession

Your app can’t access the device because another session is currently using it.

case deviceInUseByAnotherApplication

Your app can’t access the device because another app is currently using it.

case deviceLockedForConfigurationByAnotherProcess

Your app can’t change device settings because another process currently controls the device.

case deviceNotConnected

You app can’t access the device because it isn’t connected.

case deviceWasDisconnected

A previously connected device is no longer accessible.

case diskFull

Recording stopped because the disk is full.

case displayWasDisabled

Screen capture failed because the display was inactive.

case encodeFailed

The system couldn’t encode the media data.

case encoderNotFound

The requested encoder isn’t found.

case encoderTemporarilyUnavailable

An appropriate encoder isn’t currently available.

case exportFailed

The requested export operation failed.

case externalPlaybackNotSupportedForAsset

The current asset doesn’t support playback.

case failedToLoadMediaData

The system can’t load the requested media data.

case failedToLoadSampleData

The system can’t load the requested sample data.

case failedToParse

The system can’t parse the media.

case fileAlreadyExists

A file with the same name exists at the location and you can’t overwrite it.

case fileFailedToParse

The file is corrupt or in an unrecognized format.

case fileFormatNotRecognized

The system can’t open the file because it’s in an unrecognized format.

case fileTypeDoesNotSupportSampleReferences

The file type doesn’t support sample references.

case formatUnsupported

The current asset format isn’t supported.

case incompatibleAsset

You can’t display the media because the device isn’t capable of playing the content.

case incorrectlyConfigured

The system is incorrectly configured for the requested operation.

case invalidCompositionTrackSegmentDuration

You can’t add the source media because its duration in the destination is invalid.

case invalidCompositionTrackSegmentSourceDuration

You can’t add the source media because it has no duration.

case invalidCompositionTrackSegmentSourceStartTime

You can’t add the source media because its start time in the destination is invalid.

case invalidOutputURLPathExtension

The path extension of the output URL is invalid.

case invalidSampleCursor

An invalid sample cursor produced an error.

case invalidSourceMedia

The system couldn’t read the source media.

case invalidVideoComposition

You attempted to present an unsupported video composition.

case malformedDepth

The depth data isn’t properly structured.

case maximumDurationReached

The recording stopped because it reached the file’s maximum duration.

case maximumFileSizeReached

The recording stopped because it reached the file’s maximum size.

case maximumNumberOfSamplesForFileFormatReached

The recording stopped because it reached the file’s maximum number of samples.

case maximumStillImageCaptureRequestsExceeded

Your app can’t take a photo because there are too many unfinished photo capture requests.

case mediaChanged

Recording stopped because the format of the source media changed.

case mediaDiscontinuity

Recording stopped because there was an interruption in the input media.

case mediaServicesWereReset

The system couldn’t perform the operation because media services were unavailable.

case noCompatibleAlternatesForExternalDisplay

The system found no compatible external displays.

case noDataCaptured

The recording failed because the system received no data.

case noImageAtTime

No image is available in the media at the indicated time.

case noLongerPlayable

The asset is no longer playable.

case noSourceTrack

The asset doesn’t contain a source track.

case operationCancelled

The asset handled a request to cancel loading a property value asynchronously.

case operationInterrupted

An interruption occurred while performing a reading or writing operation.

case operationNotAllowed

The requested operation isn’t allowed.

case operationNotSupportedForAsset

Your app attempted to perform an unsupported operation with the asset.

case operationNotSupportedForPreset

Your app attempted to perform an unsupported operation for the current preset.

case outOfMemory

The operation couldn’t finish because there isn’t enough memory available to process the media.

case recordingAlreadyInProgress

Your app attempted to start recording a movie file while an existing recording is underway.

case referenceForbiddenByReferencePolicy

The current reference restrictions prevent the system from loading referenced media.

case rosettaNotInstalled

The system doesn’t have Rosetta installed and can’t perform the requested operation.

case sandboxExtensionDenied

The system denied issuing the sandbox extension.

case screenCaptureFailed

An unexpected problem occurred that prevented screen capture.

case segmentStartedWithNonSyncSample

The operation attempted to write a new MPEG-4 segment that didn’t start with a sync sample.

case serverIncorrectlyConfigured

The configuration of the HTTP server that streams the media resource isn’t correct.

case sessionConfigurationChanged

Recording stopped because the configuration of media sources and destinations changed.

case sessionHardwareCostOverage

Your app requested too many camera hardware resources.

case sessionNotRunning

The recording couldn’t start because the session isn’t running.

case sessionWasInterrupted

The recording stopped because the system interrupted the audio session.

case toneMappingFailed

The requested tone mapping failed.

case torchLevelUnavailable

The specified torch level is valid but currently unavailable, possibly due to overheating.

case undecodableMediaData

The system couldn’t decode the media data.

case unknown

An unknown error occurred.

case unsupportedDeviceActiveFormat

The capture session doesn’t support the camera device’s active format.

case unsupportedOutputSettings

Your app requested unsupported output settings.

case videoCompositorFailed

The compositor couldn’t composite video frames.

case deviceIsNotAvailableInBackground

You attempted to start a capture session in the background, which isn’t allowed in iOS.

Deprecated

### Enumeration Cases

case mediaExtensionConflict

case mediaExtensionDisabled

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

