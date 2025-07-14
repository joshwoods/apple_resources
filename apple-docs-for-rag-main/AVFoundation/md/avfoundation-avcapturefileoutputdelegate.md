

- AVFoundation
-  AVCaptureFileOutputDelegate 

Protocol

# AVCaptureFileOutputDelegate

Methods for monitoring or controlling the output of a media file capture.

macOS 10.7+

``` source
protocol AVCaptureFileOutputDelegate : NSObjectProtocol
```

## Overview

The `AVCaptureFileOutputDelegate` protocol defines an interface for delegates of an AVCaptureFileOutput object to monitor and control recordings along exact sample boundaries.

## Topics

### Sample Processing

func fileOutputShouldProvideSampleAccurateRecordingStart(AVCaptureFileOutput) -> Bool

Allows a client to opt in to frame accurate recording in fileOutput(_:didOutputSampleBuffer:from:).

**Required**

func fileOutput(AVCaptureFileOutput, didOutputSampleBuffer: CMSampleBuffer, from: AVCaptureConnection)

Gives the delegate the opportunity to inspect samples as they are received by the output and start and stop recording at exact times.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### File capture

Recording movies in alternative formats

Change the default format for capturing movie files.

class AVCaptureMovieFileOutput

A capture output that records video and audio to a QuickTime movie file.

class AVCaptureAudioFileOutput

A capture output that records audio and saves the recorded audio to a file.

class AVCaptureFileOutput

The abstract superclass for capture outputs that can record captured data to a file.

protocol AVCaptureFileOutputRecordingDelegate

Methods for responding to events that occur while recording captured media to a file.

