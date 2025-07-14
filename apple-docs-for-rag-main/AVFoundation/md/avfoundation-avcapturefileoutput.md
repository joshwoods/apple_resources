

- AVFoundation
-  AVCaptureFileOutput 

Class

# AVCaptureFileOutput

The abstract superclass for capture outputs that can record captured data to a file.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
class AVCaptureFileOutput
```

## Topics

### Setting File Output Properties

var delegate: (any AVCaptureFileOutputDelegate)?

The delegate object for the capture file output.

var maxRecordedDuration: CMTime

The longest duration allowed for the recording.

var maxRecordedFileSize: Int64

The maximum size, in bytes, of the data that should be recorded by the receiver.

var minFreeDiskSpaceLimit: Int64

The minimum amount of free space, in bytes, required for recording to continue on a given volume.

var outputFileURL: URL?

The URL to which output is directed.

var recordedDuration: CMTime

Indicates the duration of the media recorded to the current output file.

var recordedFileSize: Int64

Indicates the size, in bytes, of the data recorded to the current output file.

var isRecording: Bool

Indicates whether recording is in progress.

var isRecordingPaused: Bool

Indicates whether recording to the current output file is paused.

### Starting, Stopping, Pausing, and Resuming Playback

func startRecording(to: URL, recordingDelegate: any AVCaptureFileOutputRecordingDelegate)

Starts recording media to the specified output URL.

func stopRecording()

Tells the receiver to stop recording to the current file.

func pauseRecording()

Pauses recording to the current output file.

func resumeRecording()

Resumes recording to the current output file after it was previously paused using pauseRecording().

## Relationships

### Inherits From

- AVCaptureOutput

### Inherited By

- AVCaptureAudioFileOutput
- AVCaptureMovieFileOutput

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

class AVCaptureMovieFileOutput

A capture output that records video and audio to a QuickTime movie file.

class AVCaptureAudioFileOutput

A capture output that records audio and saves the recorded audio to a file.

protocol AVCaptureFileOutputDelegate

Methods for monitoring or controlling the output of a media file capture.

protocol AVCaptureFileOutputRecordingDelegate

Methods for responding to events that occur while recording captured media to a file.

