

- AVFoundation
-  AVCaptureAudioFileOutput 

Class

# AVCaptureAudioFileOutput

A capture output that records audio and saves the recorded audio to a file.

macOS 10.7+

``` source
class AVCaptureAudioFileOutput
```

## Overview

`AVCaptureAudioFileOutput` implements the complete file recording interface declared by AVCaptureFileOutput for writing media data to audio files. In addition, you can configure options specific to the audio file formats, including writing metadata collections to each file and specifying audio encoding options. `AVCaptureAudioFileOutput` does not, however, support startRecording(to:recordingDelegate:)—use startRecording(to:outputFileType:recordingDelegate:) instead.

## Topics

### Discovering Supported Types

class func availableOutputFileTypes() -> [AVFileType]

Returns an array containing UTIs identifying the file types `AVCaptureAudioFileOutput` can write.

### Starting a Recording

func startRecording(to: URL, outputFileType: AVFileType, recordingDelegate: any AVCaptureFileOutputRecordingDelegate)

Tells the receiver to start recording to a new file of the specified format, and specifies a delegate that will be notified when recording is finished.

### Configuring Output

var audioSettings: [String : Any]?

The settings used to decode or re-encode audio before it is output by the receiver.

var metadata: [AVMetadataItem]

A collection of metadata to be written to the receiver’s output files.

### Creating Output

init()

Creates a new audio file output.

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

class AVCaptureMovieFileOutput

A capture output that records video and audio to a QuickTime movie file.

class AVCaptureFileOutput

The abstract superclass for capture outputs that can record captured data to a file.

protocol AVCaptureFileOutputDelegate

Methods for monitoring or controlling the output of a media file capture.

protocol AVCaptureFileOutputRecordingDelegate

Methods for responding to events that occur while recording captured media to a file.

