

- ReplayKit
-  RPRecordingErrorCode 

Enumeration

# RPRecordingErrorCode

The ReplayKit error domain codes.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 11.0+tvOS 9.0+visionOS 1.0+

``` source
enum RPRecordingErrorCode
```

## Topics

### Errors

case activePhoneCall

Unable to record due to an active phone call.

case attemptToStartInRecordingState

Attempted to start a recording that’s already in a recording state.

case attemptToStopNonRecording

Attempted to stop a recording that’s not in a recording state.

case broadcastInvalidSession

Attempted to start a broadcast without a prior session.

case broadcastSetupFailed

The broadcast set up failed.

case carPlay

Failed to start recording because CarPlay is active.

case codeSuccessful

Successfully saved the recording to the Camera Roll.

case contentResize

Recording interrupted by multitasking and content resizing.

case disabled

Recording disabled via parental controls.

case entitlements

Recording failed due to missing entitlements.

case failed

Recording error occurred.

case failedApplicationConnectionInterrupted

The recording failed because the app’s connection was interrupted.

case failedApplicationConnectionInvalid

The recording failed because the app’s connection is invalid.

case failedAssetWriterExportCanceled

The recording failed because the user canceled the export.

case failedAssetWriterExportFailed

The recording failed due to an error exporting the movie.

case failedAssetWriterFailedToSave

The recording failed due to an asset writer failure.

case failedAssetWriterInWrongState

The recording failed because the asset writer is in an invalid state.

case failedIncorrectTimeStamps

The recording failed due to malformed start and end time intervals.

case failedMediaServicesFailure

The recording failed due to a mediaservices daemon failure.

case failedNoAssetWriter

The recording failed because there is no asset writer available.

case failedNoMatchingApplicationContext

The context identifier doesn’t match the app identifier.

case failedToObtainURL

The recording failed due to a failure to obtain the URL.

case failedToProcessFirstSample

The recording failed because the asset writer failed to process the first media sample.

case failedToRemoveFile

The recording failed because the temporary file wasn’t removed.

case failedToStartCaptureStack

The system failed to configure the app for A/V recording.

case failedToStart

Recording failed to start.

case failedToSave

The recording failed to save.

case filePermissions

The recording failed due to a file permission error.

case insufficientStorage

Not enough storage available on the device.

case interrupted

Recording interrupted by another app.

case invalidParameter

The recording failed because of an invalid parameter.

case photoFailure

Failed saving the video the Camera Roll.

case recordingInvalidSession

Attempted to start an invalid recording session.

case systemDormancy

Recording forced to end by the user pressing the power button.

case unknown

Error cause unknown.

case userDeclined

User declined recording request.

case videoMixingFailure

The recording failed due to an A/V mixing failure.

### Enumeration Cases

case exportClipToURLInProgress

### Initializers

init?(rawValue: Int)

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Errors

RPRecordingErrorDomain

The ReplayKit framework error domain.

