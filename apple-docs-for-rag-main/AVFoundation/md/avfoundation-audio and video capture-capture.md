

- AVFoundation
-  Audio and video capture 

API Collection

# Audio and video capture

Capture audio and video directly to media files, or capture streams of media for direct access to media sample buffers.

## Topics

### File capture

Recording movies in alternative formats

Change the default format for capturing movie files.

class AVCaptureMovieFileOutput

A capture output that records video and audio to a QuickTime movie file.

class AVCaptureAudioFileOutput

A capture output that records audio and saves the recorded audio to a file.

class AVCaptureFileOutput

The abstract superclass for capture outputs that can record captured data to a file.

protocol AVCaptureFileOutputDelegate

Methods for monitoring or controlling the output of a media file capture.

protocol AVCaptureFileOutputRecordingDelegate

Methods for responding to events that occur while recording captured media to a file.

### Stream capture

class AVCaptureVideoDataOutput

A capture output that records video and provides access to video frames for processing.

class AVCaptureAudioDataOutput

A capture output that records audio and provides access to audio sample buffers as they are recorded.

### Mac screen capture

class AVCaptureScreenInput

A capture input for recording from a screen in macOS.

## See Also

### Capture

Capture setup

Configure built-in cameras and microphones, and external capture devices, for media capture.

Photo capture

Capture high-quality still images, Live Photos, and supporting photo data.

Additional data capture

Capture additional data including depth and metadata, and synchronize capture from multiple outputs.

