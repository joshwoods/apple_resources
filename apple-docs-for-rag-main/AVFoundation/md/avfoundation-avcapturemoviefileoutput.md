

- AVFoundation
-  AVCaptureMovieFileOutput 

Class

# AVCaptureMovieFileOutput

A capture output that records video and audio to a QuickTime movie file.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
class AVCaptureMovieFileOutput
```

## Mentioned in 

Recording movies in alternative formats

Setting Up a Capture Session

## Overview

A movie file output provides a complete file recording interface for writing media data to QuickTime movie files. It includes the ability to configure QuickTime-specific options, including writing metadata collections to each file, specify media encoding options for each track, and specify the interval at which it writes movie fragments.

## Topics

### Creating a movie file output

init()

Creates a new of movie file output.

### Configuring movies

var movieFragmentInterval: CMTime

The number of seconds of output that are written per fragment.

var metadata: [AVMetadataItem]?

The metadata for the output file.

### Managing output settings

func supportedOutputSettingsKeys(for: AVCaptureConnection) -> [String]

Returns a list of supported keys to use in the output settings dictionary.

func outputSettings(for: AVCaptureConnection) -> [String : Any]

Returns the settings the output uses to encode media from the specified connection.

func setOutputSettings([String : Any]?, for: AVCaptureConnection)

Sets the options the output uses to encode media from the given connection while recording.

var availableVideoCodecTypes: [AVVideoCodecType]

The video codecs types the output supports for recording movie files.

### Enabling spatial capture

var isSpatialVideoCaptureSupported: Bool

A Boolean value that indicates whether a movie file output supports capturing spatial videos.

var isSpatialVideoCaptureEnabled: Bool

A Boolean value that indicates whether a movie file output captures spatial videos.

### Setting orientation

func recordsVideoOrientationAndMirroringChangesAsMetadataTrack(for: AVCaptureConnection) -> Bool

A Boolean value that indicates whether the movie file output records video orientation and mirroring information as a metadata track.

func setRecordsVideoOrientationAndMirroringChangesAsMetadataTrack(Bool, for: AVCaptureConnection)

Sets whether the movie file output creates a timed metadata track to capture changes to the connection’s video orientation and mirroring.

### Restricting camera switching

var isPrimaryConstituentDeviceSwitchingBehaviorForRecordingEnabled: Bool

A Boolean value that indicates whether to restrict constituent device switching behavior during recording.

func setPrimaryConstituentDeviceSwitchingBehaviorForRecording(AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior, restrictedSwitchingBehaviorConditions: AVCaptureDevice.PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions)

Sets the camera switching behavior to use during recording.

var primaryConstituentDeviceSwitchingBehaviorForRecording: AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior

The camera switching behavior to use for recording.

var primaryConstituentDeviceRestrictedSwitchingBehaviorConditionsForRecording: AVCaptureDevice.PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions

The conditions during which camera switching may occur while recording.

## Relationships

### Inherits From

- AVCaptureFileOutput

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### File capture

Recording movies in alternative formats

Change the default format for capturing movie files.

class AVCaptureAudioFileOutput

A capture output that records audio and saves the recorded audio to a file.

class AVCaptureFileOutput

The abstract superclass for capture outputs that can record captured data to a file.

protocol AVCaptureFileOutputDelegate

Methods for monitoring or controlling the output of a media file capture.

protocol AVCaptureFileOutputRecordingDelegate

Methods for responding to events that occur while recording captured media to a file.

