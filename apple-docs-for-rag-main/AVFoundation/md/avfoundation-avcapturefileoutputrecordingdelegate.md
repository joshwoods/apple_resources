

- AVFoundation
-  AVCaptureFileOutputRecordingDelegate 

Protocol

# AVCaptureFileOutputRecordingDelegate

Methods for responding to events that occur while recording captured media to a file.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
protocol AVCaptureFileOutputRecordingDelegate : NSObjectProtocol
```

## Overview

Defines an interface for delegates of AVCaptureFileOutput to respond to events that occur in the process of recording a single file.

The delegate of an `AVCaptureFileOutput` object must adopt the `AVCaptureFileOutputRecordingDelegate` protocol.

## Topics

### Delegate Methods

func fileOutput(AVCaptureFileOutput, didStartRecordingTo: URL, from: [AVCaptureConnection])

Informs the delegate when the output has started writing to a file.

func fileOutput(AVCaptureFileOutput, willFinishRecordingTo: URL, from: [AVCaptureConnection], error: (any Error)?)

Informs the delegate when the output will stop writing new samples to a file.

func fileOutput(AVCaptureFileOutput, didFinishRecordingTo: URL, from: [AVCaptureConnection], error: (any Error)?)

Informs the delegate when all pending data has been written to an output file.

**Required**

func fileOutput(AVCaptureFileOutput, didPauseRecordingTo: URL, from: [AVCaptureConnection])

Called whenever the output is recording to a file and successfully pauses the recording at the request of a client.

func fileOutput(AVCaptureFileOutput, didResumeRecordingTo: URL, from: [AVCaptureConnection])

Called whenever the output, at the request of the client, successfully resumes a file recording that was paused.

### Instance Methods

func fileOutput(AVCaptureFileOutput, didStartRecordingTo: URL, startPTS: CMTime, from: [AVCaptureConnection])

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

protocol AVCaptureFileOutputDelegate

Methods for monitoring or controlling the output of a media file capture.

